# <a name="user-delta"></a><span data-ttu-id="a629e-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="a629e-101">user: delta</span></span>

<span data-ttu-id="a629e-102">Get を新しく作成するには、更新、または全体のユーザーのコレクションのすべての読み取りを実行することがなくユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="a629e-102">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="a629e-103">詳細については、[変更履歴の記録](../../../concepts/delta_query_overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a629e-103">See [Track changes](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a629e-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a629e-104">Permissions</span></span>

<span data-ttu-id="a629e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a629e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="a629e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a629e-107">Permission type</span></span>      | <span data-ttu-id="a629e-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a629e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a629e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a629e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a629e-110">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a629e-110">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a629e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a629e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a629e-112">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a629e-112">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="a629e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a629e-113">Application</span></span> | <span data-ttu-id="a629e-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a629e-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a629e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a629e-115">HTTP request</span></span>

<span data-ttu-id="a629e-116">変更の追跡を開始するには、ユーザー リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="a629e-116">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a629e-117">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a629e-117">Query parameters</span></span>

<span data-ttu-id="a629e-118">ユーザーの変更の追跡と、一連の 1 つまたは複数の**delta**関数の呼び出しが発生します。</span><span class="sxs-lookup"><span data-stu-id="a629e-118">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="a629e-119">任意のクエリ パラメーターを使用する場合 (以外の`$deltatoken`と`$skiptoken`)、**デルタ**の初期要求で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a629e-119">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="a629e-120">Microsoft Graph が自動的に任意指定のパラメーターをエンコードのトークンの部分に、`nextLink`または`deltaLink`の応答で提供される URL です。</span><span class="sxs-lookup"><span data-stu-id="a629e-120">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="a629e-121">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="a629e-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="a629e-122">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="a629e-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a629e-123">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a629e-123">Query parameter</span></span>      | <span data-ttu-id="a629e-124">種類</span><span class="sxs-lookup"><span data-stu-id="a629e-124">Type</span></span>   |<span data-ttu-id="a629e-125">説明</span><span class="sxs-lookup"><span data-stu-id="a629e-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a629e-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a629e-126">$deltatoken</span></span> | <span data-ttu-id="a629e-127">文字列</span><span class="sxs-lookup"><span data-stu-id="a629e-127">string</span></span> | <span data-ttu-id="a629e-p104">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="a629e-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a629e-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a629e-130">$skiptoken</span></span> | <span data-ttu-id="a629e-131">文字列</span><span class="sxs-lookup"><span data-stu-id="a629e-131">string</span></span> | <span data-ttu-id="a629e-132">前の**デルタ**関数の `nextLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="a629e-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="a629e-133">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a629e-133">OData query parameters</span></span>

<span data-ttu-id="a629e-134">このメソッドは、応答をカスタマイズするためのオプションの OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="a629e-134">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="a629e-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。*Id* プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="a629e-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="a629e-137">サポートが制限されて`$filter`。</span><span class="sxs-lookup"><span data-stu-id="a629e-137">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="a629e-138">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="a629e-138">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="a629e-139">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="a629e-139">You can filter multiple objects.</span></span> <span data-ttu-id="a629e-140">たとえば、`https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'` などです。</span><span class="sxs-lookup"><span data-stu-id="a629e-140">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="a629e-141">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="a629e-141">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a629e-142">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a629e-142">Request headers</span></span>
| <span data-ttu-id="a629e-143">名前</span><span class="sxs-lookup"><span data-stu-id="a629e-143">Name</span></span>       | <span data-ttu-id="a629e-144">説明</span><span class="sxs-lookup"><span data-stu-id="a629e-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a629e-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="a629e-145">Authorization</span></span>  | <span data-ttu-id="a629e-146">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="a629e-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="a629e-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a629e-147">Content-Type</span></span>  | <span data-ttu-id="a629e-148">application/json</span><span class="sxs-lookup"><span data-stu-id="a629e-148">application/json</span></span> |
| <span data-ttu-id="a629e-149">Prefer</span><span class="sxs-lookup"><span data-stu-id="a629e-149">Prefer</span></span> | <span data-ttu-id="a629e-150">返す最小 =</span><span class="sxs-lookup"><span data-stu-id="a629e-150">return=minimal</span></span> <br><br><span data-ttu-id="a629e-151">このヘッダーを指定する要求を使用すると、`deltaLink`最後のラウンド以降に変更されたオブジェクトのプロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="a629e-151">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="a629e-152">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a629e-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a629e-153">要求本文</span><span class="sxs-lookup"><span data-stu-id="a629e-153">Request body</span></span>
<span data-ttu-id="a629e-154">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a629e-154">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="a629e-155">応答</span><span class="sxs-lookup"><span data-stu-id="a629e-155">Response</span></span>

<span data-ttu-id="a629e-156">かどうかは成功すると、このメソッドを返します`200 OK`応答の本体で応答コードと[ユーザー](../resources/user.md)コレクションのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a629e-156">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="a629e-157">応答にも含まれています、`nextLink`の URL、または`deltaLink`URL です。</span><span class="sxs-lookup"><span data-stu-id="a629e-157">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="a629e-158">場合、`nextLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="a629e-158">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="a629e-159">これは、他のページのセッションで取得するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="a629e-159">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="a629e-160">アプリケーションの継続を使用して要求を作成する、`nextLink`までの URL を`deltaLink`URL が応答に含まれています。</span><span class="sxs-lookup"><span data-stu-id="a629e-160">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="a629e-161">応答には、同じ一連最初のデルタ ・ クエリ要求のようにプロパティにはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a629e-161">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="a629e-162">これにより、デルタ ・ サイクルを開始するときに、オブジェクトのすべての現在の状態をキャプチャすることができます。</span><span class="sxs-lookup"><span data-stu-id="a629e-162">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="a629e-163">場合、`deltaLink`の URL が返されます。</span><span class="sxs-lookup"><span data-stu-id="a629e-163">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="a629e-164">これは、返されるリソースの既存の状態に関するデータがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="a629e-164">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="a629e-165">保存し、使用して、`deltaLink`について学習するための URL は次のラウンドでリソースを変更します。</span><span class="sxs-lookup"><span data-stu-id="a629e-165">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="a629e-166">指定の選択肢がある場合、`Prefer:return=minimal`時間以降に変更されたプロパティのみの応答の値に追加する、ヘッダー、`deltaLink`が発行されました。</span><span class="sxs-lookup"><span data-stu-id="a629e-166">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="a629e-167">既定値: は、最初のデルタ ・ リクエストと同じプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="a629e-167">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="a629e-168">既定では、要求を使用して、`deltaLink`または`nextLink`次のように最初のデルタ ・ クエリで選択したのと同じプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="a629e-168">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="a629e-169">プロパティが変更された場合は、JSON 応答のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="a629e-169">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="a629e-170">プロパティは空の値に設定されている場合、は、プロパティの値として null を返します。</span><span class="sxs-lookup"><span data-stu-id="a629e-170">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="a629e-171">プロパティが変更されていない場合は、null 値を返します。</span><span class="sxs-lookup"><span data-stu-id="a629e-171">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="a629e-172">**注:** 上の動作では変更されていないプロパティと 1 つに変更されたことの間で区別するために、`null`の値です。</span><span class="sxs-lookup"><span data-stu-id="a629e-172">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="a629e-173">次の[2 番目の例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a629e-173">See the [second example](#request-2) below.</span></span> <span data-ttu-id="a629e-174">これは重要ですが、次のセクションで説明されている代替の動作を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a629e-174">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="a629e-175">: 別の方法が変更されたプロパティのみを返す</span><span class="sxs-lookup"><span data-stu-id="a629e-175">Alternative: return only the changed properties</span></span>

<span data-ttu-id="a629e-176">オプションの要求ヘッダーでは - を追加する`prefer:return=minimal`の次の動作の結果します。</span><span class="sxs-lookup"><span data-stu-id="a629e-176">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="a629e-177">プロパティが変更された場合は、JSON 応答のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="a629e-177">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="a629e-178">プロパティは空の値に設定されている場合、は、プロパティの値として null を返します。</span><span class="sxs-lookup"><span data-stu-id="a629e-178">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="a629e-179">プロパティが変更されていない場合は、JSON 応答のプロパティを含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a629e-179">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="a629e-180">(既定の動作と異なります)</span><span class="sxs-lookup"><span data-stu-id="a629e-180">(Different from the default behavior.)</span></span>

> <span data-ttu-id="a629e-181">**注:** ヘッダーを追加することができます、`deltaLink`デルタ ・ サイクルの時間内の任意の時点で要求します。</span><span class="sxs-lookup"><span data-stu-id="a629e-181">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="a629e-182">ヘッダーの応答に含まれるプロパティのセットにのみ影響し、デルタ ・ クエリを実行する方法には影響しません。</span><span class="sxs-lookup"><span data-stu-id="a629e-182">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="a629e-183">次の[3 番目の例](#request-3)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a629e-183">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="a629e-184">例</span><span class="sxs-lookup"><span data-stu-id="a629e-184">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="a629e-185">要求 1</span><span class="sxs-lookup"><span data-stu-id="a629e-185">Request 1</span></span>

<span data-ttu-id="a629e-186">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a629e-186">The following is an example of the request.</span></span> <span data-ttu-id="a629e-187">ありません`$select`パラメーター、プロパティの既定のセットが追跡され、返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="a629e-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="a629e-188">応答 1</span><span class="sxs-lookup"><span data-stu-id="a629e-188">Response 1</span></span>

<span data-ttu-id="a629e-189">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="a629e-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="a629e-p116">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a629e-p116">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="a629e-192">要求 2</span><span class="sxs-lookup"><span data-stu-id="a629e-192">Request 2</span></span>

<span data-ttu-id="a629e-193">次の使用例は、変更の追跡、応答の既定の動作で 3 つのプロパティを選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a629e-193">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="a629e-194">応答 2</span><span class="sxs-lookup"><span data-stu-id="a629e-194">Response 2</span></span>

<span data-ttu-id="a629e-195">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="a629e-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="a629e-196">注意してください`jobTitle`と`mobilePhone`の値を持つ`null`可能性がありますが変更されていない、または、空の値に設定されていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="a629e-196">Note that `jobTitle` and `mobilePhone` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null,
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="a629e-197">要求 3</span><span class="sxs-lookup"><span data-stu-id="a629e-197">Request 3</span></span>

<span data-ttu-id="a629e-198">次の使用例は、3 つのプロパティの変更履歴の記録を最小限に抑える別の応答の動作を選択する最初の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a629e-198">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="a629e-199">応答 3</span><span class="sxs-lookup"><span data-stu-id="a629e-199">Response 3</span></span>

<span data-ttu-id="a629e-200">使用すると、次の応答の例では`deltaLink`クエリの初期化から取得します。</span><span class="sxs-lookup"><span data-stu-id="a629e-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="a629e-201">なお、`mobilePhone`プロパティが含まれていないことを意味するは、前回のデルタ ・ クエリは変更されていません。`displayName`と`jobTitle`は、値が変更されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="a629e-201">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="a629e-202">[グラフ データの変更を追跡するためにデルタのクエリを使用します](../../../concepts/delta_query_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a629e-202">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="a629e-203">[ユーザーの増分の変更を取得](../../../concepts/delta_query_users.md)します。</span><span class="sxs-lookup"><span data-stu-id="a629e-203">[Get incremental changes for users](../../../concepts/delta_query_users.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->