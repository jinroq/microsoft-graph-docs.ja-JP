# <a name="group-delta"></a><span data-ttu-id="dab21-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="dab21-101">group: delta</span></span>
<span data-ttu-id="dab21-102">Get を新しく作成するには、更新、またはグループ メンバーシップの変更を含むグループ全体のコレクションのすべての読み取りを実行しなくても、グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="dab21-102">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="dab21-103">詳細については、[デルタのクエリを使用する](../../../concepts/delta_query_overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dab21-103">See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="dab21-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dab21-104">Permissions</span></span>

<span data-ttu-id="dab21-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dab21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dab21-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dab21-107">Permission type</span></span>      | <span data-ttu-id="dab21-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dab21-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dab21-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dab21-109">Delegated (work or school account)</span></span> | <span data-ttu-id="dab21-110">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab21-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dab21-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dab21-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dab21-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dab21-112">Not supported.</span></span>    |
|<span data-ttu-id="dab21-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dab21-113">Application</span></span> | <span data-ttu-id="dab21-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab21-114">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dab21-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dab21-115">HTTP request</span></span>

<span data-ttu-id="dab21-116">変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="dab21-116">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="dab21-117">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dab21-117">Query parameters</span></span>

<span data-ttu-id="dab21-p103">グループで変更の追跡を実行するときには、1 つまたは複数の **delta** 関数の呼び出しが必要になります。クエリ パラメーター (`$deltatoken` および `$skiptoken` 以外) を使用する場合は、そのパラメーターを最初の **delta** 要求に指定する必要があります。指定されたパラメーターは、Microsoft Graph を使って自動的にエンコードされ、応答の `nextLink` または `deltaLink` URL のトークン部分として指定されます。</span><span class="sxs-lookup"><span data-stu-id="dab21-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="dab21-121">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="dab21-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="dab21-122">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="dab21-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="dab21-123">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dab21-123">Query parameter</span></span> | <span data-ttu-id="dab21-124">種類</span><span class="sxs-lookup"><span data-stu-id="dab21-124">Type</span></span>  |<span data-ttu-id="dab21-125">説明</span><span class="sxs-lookup"><span data-stu-id="dab21-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dab21-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="dab21-126">$deltatoken</span></span> | <span data-ttu-id="dab21-127">文字列</span><span class="sxs-lookup"><span data-stu-id="dab21-127">string</span></span> | <span data-ttu-id="dab21-p104">同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="dab21-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="dab21-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="dab21-130">$skiptoken</span></span> | <span data-ttu-id="dab21-131">文字列</span><span class="sxs-lookup"><span data-stu-id="dab21-131">string</span></span> | <span data-ttu-id="dab21-132">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="dab21-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="dab21-133">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dab21-133">OData query parameters</span></span>

<span data-ttu-id="dab21-134">このメソッドは、応答をカスタマイズするためのオプションの OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="dab21-134">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="dab21-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="dab21-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="dab21-137">使用することができます`$expand=members`のメンバーシップの変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="dab21-137">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="dab21-138">サポートが制限されて`$filter`。</span><span class="sxs-lookup"><span data-stu-id="dab21-138">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="dab21-139">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="dab21-139">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="dab21-140">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="dab21-140">You can filter multiple objects.</span></span> <span data-ttu-id="dab21-141">たとえば、`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="dab21-141">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="dab21-142">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="dab21-142">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dab21-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dab21-143">Request headers</span></span>

| <span data-ttu-id="dab21-144">名前</span><span class="sxs-lookup"><span data-stu-id="dab21-144">Name</span></span>       | <span data-ttu-id="dab21-145">説明</span><span class="sxs-lookup"><span data-stu-id="dab21-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dab21-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="dab21-146">Authorization</span></span>  | <span data-ttu-id="dab21-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="dab21-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="dab21-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dab21-148">Content-Type</span></span>  | <span data-ttu-id="dab21-149">application/json</span><span class="sxs-lookup"><span data-stu-id="dab21-149">application/json</span></span> |
| <span data-ttu-id="dab21-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="dab21-150">Prefer</span></span> | <span data-ttu-id="dab21-151">返す最小 =</span><span class="sxs-lookup"><span data-stu-id="dab21-151">return=minimal</span></span> <br><br><span data-ttu-id="dab21-152">このヘッダーを指定する要求を使用すると、`deltaLink`最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="dab21-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="dab21-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="dab21-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dab21-154">要求本文</span><span class="sxs-lookup"><span data-stu-id="dab21-154">Request body</span></span>

<span data-ttu-id="dab21-155">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dab21-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="dab21-156">応答</span><span class="sxs-lookup"><span data-stu-id="dab21-156">Response</span></span>

<span data-ttu-id="dab21-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dab21-157">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="dab21-158">応答には、次のいずれかの状態のトークンも含まれています、`nextLink`の URL、または`deltaLink`URL です。</span><span class="sxs-lookup"><span data-stu-id="dab21-158">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="dab21-159">場合、`nextLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="dab21-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="dab21-160">これは、他のページのセッションで取得するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="dab21-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="dab21-161">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="dab21-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="dab21-162">応答には、同じ一連最初のデルタ ・ クエリ要求のようにプロパティにはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dab21-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="dab21-163">これにより、デルタ ・ サイクルを開始するときに、オブジェクトのすべての現在の状態をキャプチャすることができます。</span><span class="sxs-lookup"><span data-stu-id="dab21-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="dab21-164">場合、`deltaLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="dab21-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="dab21-165">これは、返されるリソースの既存の状態に関するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="dab21-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="dab21-166">保存し、使用して、`deltaLink`について学習するための URL は次のラウンドでリソースを変更します。</span><span class="sxs-lookup"><span data-stu-id="dab21-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="dab21-167">指定の選択肢がある場合、`Prefer:return=minimal`時間以降に変更されたプロパティのみの応答の値に追加する、ヘッダー、`deltaLink`が発行されました。</span><span class="sxs-lookup"><span data-stu-id="dab21-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="dab21-168">既定値: は、最初のデルタ ・ リクエストと同じプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="dab21-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="dab21-169">既定では、要求を使用して、`deltaLink`または`nextLink`次のように最初のデルタ ・ クエリで選択したのと同じプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="dab21-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="dab21-170">プロパティが変更された場合は、JSON 応答のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="dab21-170">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="dab21-171">プロパティは空の値に設定されている場合、は、プロパティの値として null を返します。</span><span class="sxs-lookup"><span data-stu-id="dab21-171">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="dab21-172">プロパティが変更されていない場合は、null 値を返します。</span><span class="sxs-lookup"><span data-stu-id="dab21-172">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="dab21-173">**注:** 上の動作では変更されていないプロパティと 1 つに変更されたことの間で区別するために、`null`の値です。</span><span class="sxs-lookup"><span data-stu-id="dab21-173">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="dab21-174">次の[2 番目の例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dab21-174">See the [second example](#request-2) below.</span></span> <span data-ttu-id="dab21-175">これは重要ですが、次のセクションで説明されている代替の動作を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="dab21-175">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="dab21-176">: 別の方法が変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="dab21-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="dab21-177">オプションの要求ヘッダーでは - を追加する`prefer:return=minimal`の次の動作の結果します。</span><span class="sxs-lookup"><span data-stu-id="dab21-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="dab21-178">プロパティが変更された場合は、JSON 応答のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="dab21-178">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="dab21-179">プロパティは空の値に設定されている場合、は、プロパティの値として null を返します。</span><span class="sxs-lookup"><span data-stu-id="dab21-179">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="dab21-180">プロパティが変更されていない場合は、JSON 応答のプロパティを含めないでください。</span><span class="sxs-lookup"><span data-stu-id="dab21-180">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="dab21-181">(既定の動作と異なります)</span><span class="sxs-lookup"><span data-stu-id="dab21-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="dab21-182">**注:** ヘッダーを追加することができます、`deltaLink`デルタ ・ サイクルの時間内の任意の時点で要求します。</span><span class="sxs-lookup"><span data-stu-id="dab21-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="dab21-183">ヘッダーの応答に含まれるプロパティのセットにのみ影響し、デルタ ・ クエリを実行する方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="dab21-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="dab21-184">次の[3 番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dab21-184">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="dab21-185">例</span><span class="sxs-lookup"><span data-stu-id="dab21-185">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="dab21-186">要求 1</span><span class="sxs-lookup"><span data-stu-id="dab21-186">Request 1</span></span>

<span data-ttu-id="dab21-187">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dab21-187">The following is an example of the request.</span></span> <span data-ttu-id="dab21-188">ありません`$select`パラメーター、プロパティの既定のセットが追跡され、返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="dab21-188">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="dab21-189">応答 1</span><span class="sxs-lookup"><span data-stu-id="dab21-189">Response 1</span></span>

<span data-ttu-id="dab21-190">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="dab21-190">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="dab21-191">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="dab21-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dab21-192">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dab21-192">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="dab21-193">グループ内のメンバー オブジェクトの id が含まれている*members@delta*プロパティが存在することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="dab21-193">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="dab21-194">要求 2</span><span class="sxs-lookup"><span data-stu-id="dab21-194">Request 2</span></span>

<span data-ttu-id="dab21-195">次の使用例は、変更の追跡、応答の既定の動作で 3 つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="dab21-195">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="dab21-196">応答 2</span><span class="sxs-lookup"><span data-stu-id="dab21-196">Response 2</span></span>

<span data-ttu-id="dab21-197">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="dab21-197">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="dab21-198">注意してください`description`と`mailNickname`の値を持つ`null`可能性がありますが変更されていない、または、空の値に設定されていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="dab21-198">Note that `description` and `mailNickname` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="dab21-199">要求 3</span><span class="sxs-lookup"><span data-stu-id="dab21-199">Request 3</span></span>

<span data-ttu-id="dab21-200">次の使用例は、3 つのプロパティの変更履歴の記録を最小限に抑える別の応答の動作を選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="dab21-200">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="dab21-201">応答 3</span><span class="sxs-lookup"><span data-stu-id="dab21-201">Response 3</span></span>

<span data-ttu-id="dab21-202">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="dab21-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="dab21-203">なお、`mailNickname`プロパティが含まれていないことを意味するは、前回のデルタ ・ クエリは変更されていません。`displayName`と`description`は、値が変更されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="dab21-203">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="dab21-204">関連項目</span><span class="sxs-lookup"><span data-stu-id="dab21-204">See also</span></span>

- <span data-ttu-id="dab21-205">[グラフ データの変更を追跡するためにデルタのクエリを使用します](../../../concepts/delta_query_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="dab21-205">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="dab21-206">[グループの増分の変更を取得](../../../concepts/delta_query_groups.md)します。</span><span class="sxs-lookup"><span data-stu-id="dab21-206">[Get incremental changes for groups](../../../concepts/delta_query_groups.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
