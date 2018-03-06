# <a name="group-delta"></a><span data-ttu-id="062a1-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="062a1-101">group: delta</span></span>
<span data-ttu-id="062a1-p101">[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用すると、アプリケーションは、要求ごとにターゲット リソースをすべて読み取ることなく、新しく作成、更新、削除されたエンティティを検出できます。グループへの変更を検出するには、*デルタ*関数を使用して要求を実行します。詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="062a1-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="062a1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="062a1-105">Permissions</span></span>
<span data-ttu-id="062a1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="062a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="062a1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="062a1-108">Permission type</span></span>      | <span data-ttu-id="062a1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="062a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="062a1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="062a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="062a1-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="062a1-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="062a1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="062a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="062a1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="062a1-113">Not supported.</span></span>    |
|<span data-ttu-id="062a1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="062a1-114">Application</span></span> | <span data-ttu-id="062a1-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="062a1-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="062a1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="062a1-116">HTTP request</span></span>
<span data-ttu-id="062a1-117">変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="062a1-117">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a><span data-ttu-id="062a1-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="062a1-118">Query parameters</span></span>
<span data-ttu-id="062a1-p103">グループで変更の追跡を実行するときには、1 つまたは複数の **delta** 関数の呼び出しが必要になります。クエリ パラメーター (`$deltatoken` および `$skiptoken` 以外) を使用する場合は、そのパラメーターを最初の **delta** 要求に指定する必要があります。指定されたパラメーターは、Microsoft Graph を使って自動的にエンコードされ、応答の `nextLink` または `deltaLink` URL のトークン部分として指定されます。</span><span class="sxs-lookup"><span data-stu-id="062a1-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="062a1-122">必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="062a1-122">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="062a1-123">その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。</span><span class="sxs-lookup"><span data-stu-id="062a1-123">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="062a1-124">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="062a1-124">Query parameter</span></span>      | <span data-ttu-id="062a1-125">種類</span><span class="sxs-lookup"><span data-stu-id="062a1-125">Type</span></span>   |<span data-ttu-id="062a1-126">説明</span><span class="sxs-lookup"><span data-stu-id="062a1-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="062a1-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="062a1-127">$deltatoken</span></span> | <span data-ttu-id="062a1-128">string</span><span class="sxs-lookup"><span data-stu-id="062a1-128">string</span></span> | <span data-ttu-id="062a1-p104">同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="062a1-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="062a1-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="062a1-131">$skiptoken</span></span> | <span data-ttu-id="062a1-132">string</span><span class="sxs-lookup"><span data-stu-id="062a1-132">string</span></span> | <span data-ttu-id="062a1-133">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="062a1-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="062a1-134">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="062a1-134">Optional query parameters</span></span>
<span data-ttu-id="062a1-135">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="062a1-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="062a1-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="062a1-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="062a1-138">デルタ クエリは、グループの `$select`、`$top`、`$expand` をサポートします。</span><span class="sxs-lookup"><span data-stu-id="062a1-138">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span> 
- <span data-ttu-id="062a1-139">`$filter` と `$orderby` に対するサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="062a1-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="062a1-140">サポートされている唯一の `$filter` 式は、特定のオブジェクトでの変更を追跡する `$filter=id+eq+{value}` です。</span><span class="sxs-lookup"><span data-stu-id="062a1-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="062a1-141">複数のオブジェクトをフィルター処理することができます。</span><span class="sxs-lookup"><span data-stu-id="062a1-141">You can filter multiple objects.</span></span> <span data-ttu-id="062a1-142">たとえば、`https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff` などです。</span><span class="sxs-lookup"><span data-stu-id="062a1-142">For example: `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`.</span></span> <span data-ttu-id="062a1-143">フィルター処理されるオブジェクトには 50 の数量制限があります。</span><span class="sxs-lookup"><span data-stu-id="062a1-143">There is a limit of 50 filtered objects.</span></span>
- <span data-ttu-id="062a1-144">`$search` はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="062a1-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="062a1-145">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="062a1-145">Request headers</span></span>
| <span data-ttu-id="062a1-146">名前</span><span class="sxs-lookup"><span data-stu-id="062a1-146">Name</span></span>       | <span data-ttu-id="062a1-147">説明</span><span class="sxs-lookup"><span data-stu-id="062a1-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="062a1-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="062a1-148">Authorization</span></span>  | <span data-ttu-id="062a1-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="062a1-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="062a1-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="062a1-150">Content-Type</span></span>  | <span data-ttu-id="062a1-151">application/json</span><span class="sxs-lookup"><span data-stu-id="062a1-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="062a1-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="062a1-152">Request body</span></span>
<span data-ttu-id="062a1-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="062a1-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="062a1-154">応答</span><span class="sxs-lookup"><span data-stu-id="062a1-154">Response</span></span>
<span data-ttu-id="062a1-p107">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。応答には、状態トークン (nextLink URL や deltaLink URL) も含まれます。</span><span class="sxs-lookup"><span data-stu-id="062a1-p107">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="062a1-p108">nextLink URL が返される場合は、セッションに取得するデータの追加ページがあります。deltaLink URL が応答で返されるまで、アプリケーションは nextLink URL を使用して要求を実行し続けます。</span><span class="sxs-lookup"><span data-stu-id="062a1-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="062a1-p109">deltaLink URL が返される場合、返されるリソースの既存の状態に関するデータはありません。以降の要求では、アプリケーションは deltaLink URL を使用して、リソースへの変更点を確認します。</span><span class="sxs-lookup"><span data-stu-id="062a1-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="062a1-161">参照先:</span><span class="sxs-lookup"><span data-stu-id="062a1-161">See:</span></span></br>
- <span data-ttu-id="062a1-162">詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください</span><span class="sxs-lookup"><span data-stu-id="062a1-162">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="062a1-163">要求の例については、「[グループに対する増分の変更を取得する](../../../concepts/delta_query_groups.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="062a1-163">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for an example requests.</span></span></br>
    
## <a name="example"></a><span data-ttu-id="062a1-164">例</span><span class="sxs-lookup"><span data-stu-id="062a1-164">Example</span></span>
#### <a name="request"></a><span data-ttu-id="062a1-165">要求</span><span class="sxs-lookup"><span data-stu-id="062a1-165">Request</span></span>
<span data-ttu-id="062a1-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="062a1-166">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response"></a><span data-ttu-id="062a1-167">応答</span><span class="sxs-lookup"><span data-stu-id="062a1-167">Response</span></span>
<span data-ttu-id="062a1-168">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="062a1-168">The following is an example of the response.</span></span>
><span data-ttu-id="062a1-p110">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="062a1-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "mail": "mail-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->