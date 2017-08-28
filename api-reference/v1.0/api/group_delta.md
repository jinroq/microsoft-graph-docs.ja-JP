# <a name="group-delta"></a><span data-ttu-id="1d92b-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="1d92b-101">group: delta</span></span>

<span data-ttu-id="1d92b-p101">[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用すると、アプリケーションは、要求ごとにターゲット リソースをすべて読み取ることなく、新しく作成、更新、削除されたエンティティを検出できます。グループへの変更を検出するには、*デルタ*関数を使用して要求を実行します。詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d92b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d92b-105">Permissions</span></span>

<span data-ttu-id="1d92b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="1d92b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d92b-108">Permission type</span></span>      | <span data-ttu-id="1d92b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d92b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d92b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d92b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d92b-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d92b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d92b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d92b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d92b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d92b-113">Not supported.</span></span>    |
|<span data-ttu-id="1d92b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d92b-114">Application</span></span> | <span data-ttu-id="1d92b-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d92b-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d92b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d92b-116">HTTP request</span></span>

<span data-ttu-id="1d92b-117">変更の追跡を開始するには、グループ リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="1d92b-117">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a><span data-ttu-id="1d92b-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1d92b-118">Query parameters</span></span>

<span data-ttu-id="1d92b-p103">グループの変更を追跡すると、1 つ以上の **デルタ**関数呼び出しのラウンドが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` や `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` や `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="1d92b-124">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1d92b-124">Query parameter</span></span>      | <span data-ttu-id="1d92b-125">種類</span><span class="sxs-lookup"><span data-stu-id="1d92b-125">Type</span></span>   |<span data-ttu-id="1d92b-126">説明</span><span class="sxs-lookup"><span data-stu-id="1d92b-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d92b-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="1d92b-127">$deltatoken</span></span> | <span data-ttu-id="1d92b-128">string</span><span class="sxs-lookup"><span data-stu-id="1d92b-128">string</span></span> | <span data-ttu-id="1d92b-p104">同じグループ コレクションの前の**デルタ**関数呼び出しの `deltaLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、その変更追跡のラウンドが完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="1d92b-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="1d92b-131">$skiptoken</span></span> | <span data-ttu-id="1d92b-132">string</span><span class="sxs-lookup"><span data-stu-id="1d92b-132">string</span></span> | <span data-ttu-id="1d92b-133">前の**デルタ**関数呼び出しの `nextLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、同じグループ コレクションに追跡すべき変更が他にもあることを示します。</span><span class="sxs-lookup"><span data-stu-id="1d92b-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="1d92b-134">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1d92b-134">Optional query parameters</span></span>

<span data-ttu-id="1d92b-135">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="1d92b-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="1d92b-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="1d92b-138">デルタ クエリは、グループの `$select`、`$top`、`$expand` をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1d92b-138">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span> 
- <span data-ttu-id="1d92b-p106">`$orderby` に対するサポートには制限があります。サポートされている唯一の `$orderby` 式は、`$orderby=receivedDateTime+desc` です。`$orderby` 式を含めない場合、戻り値の順序は保証されません。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p106">There is limited support for `$orderby`: The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="1d92b-141">`$search` はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d92b-141">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d92b-142">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d92b-142">Request headers</span></span>
| <span data-ttu-id="1d92b-143">名前</span><span class="sxs-lookup"><span data-stu-id="1d92b-143">Name</span></span>       | <span data-ttu-id="1d92b-144">説明</span><span class="sxs-lookup"><span data-stu-id="1d92b-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d92b-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d92b-145">Authorization</span></span>  | <span data-ttu-id="1d92b-146">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="1d92b-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="1d92b-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d92b-147">Content-Type</span></span>  | <span data-ttu-id="1d92b-148">application/json</span><span class="sxs-lookup"><span data-stu-id="1d92b-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d92b-149">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d92b-149">Request body</span></span>
<span data-ttu-id="1d92b-150">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1d92b-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d92b-151">応答</span><span class="sxs-lookup"><span data-stu-id="1d92b-151">Response</span></span>

<span data-ttu-id="1d92b-p107">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [group](../resources/group.md) コレクション オブジェクトを返します。応答には、状態トークン (nextLink URL や deltaLink URL) も含まれます。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p107">If successful, this method returns `200, OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="1d92b-p108">nextLink URL が返される場合は、セッションに取得するデータの追加ページがあります。deltaLink URL が応答で返されるまで、アプリケーションは nextLink URL を使用して要求を実行し続けます。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="1d92b-p109">deltaLink URL が返される場合、返されるリソースの既存の状態に関するデータはありません。以降の要求では、アプリケーションは deltaLink URL を使用して、リソースへの変更点を確認します。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="1d92b-158">参照先:</span><span class="sxs-lookup"><span data-stu-id="1d92b-158">See:</span></span></br>
- <span data-ttu-id="1d92b-159">詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください</span><span class="sxs-lookup"><span data-stu-id="1d92b-159">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="1d92b-160">要求の例については、「[グループに対する増分の変更を取得する](../../../concepts/delta_query_groups.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1d92b-160">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for an example requests.</span></span></br>
    
## <a name="example"></a><span data-ttu-id="1d92b-161">例</span><span class="sxs-lookup"><span data-stu-id="1d92b-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d92b-162">要求</span><span class="sxs-lookup"><span data-stu-id="1d92b-162">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

##### <a name="response"></a><span data-ttu-id="1d92b-163">応答</span><span class="sxs-lookup"><span data-stu-id="1d92b-163">Response</span></span>
<span data-ttu-id="1d92b-p110">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d92b-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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