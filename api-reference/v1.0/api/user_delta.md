# <a name="user-delta"></a><span data-ttu-id="06adc-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="06adc-101">user: delta</span></span>

<span data-ttu-id="06adc-p101">[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用すると、アプリケーションは、要求ごとにターゲット リソースをすべて読み取ることなく、新しく作成、更新、削除されたエンティティを検出できます。ユーザーへの変更を検出するには、*デルタ*関数を使用して要求を実行します。詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="06adc-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to users, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="06adc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="06adc-105">Permissions</span></span>

<span data-ttu-id="06adc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06adc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="06adc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06adc-108">Permission type</span></span>      | <span data-ttu-id="06adc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="06adc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06adc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06adc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06adc-111">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06adc-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06adc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06adc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06adc-113">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06adc-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="06adc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06adc-114">Application</span></span> | <span data-ttu-id="06adc-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06adc-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06adc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06adc-116">HTTP request</span></span>

<span data-ttu-id="06adc-117">変更の追跡を開始するには、ユーザー リソースにデルタ関数を含む要求を実行します。</span><span class="sxs-lookup"><span data-stu-id="06adc-117">To begin tracking changes, you make a request including the delta function on the users resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="06adc-118">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="06adc-118">Query parameters</span></span>

<span data-ttu-id="06adc-p103">ユーザーの変更を追跡すると、一連の **デルタ**関数呼び出しが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` や `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` や `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。</span><span class="sxs-lookup"><span data-stu-id="06adc-p103">Tracking changes in users incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="06adc-124">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="06adc-124">Query parameter</span></span>      | <span data-ttu-id="06adc-125">種類</span><span class="sxs-lookup"><span data-stu-id="06adc-125">Type</span></span>   |<span data-ttu-id="06adc-126">説明</span><span class="sxs-lookup"><span data-stu-id="06adc-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="06adc-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="06adc-127">$deltatoken</span></span> | <span data-ttu-id="06adc-128">string</span><span class="sxs-lookup"><span data-stu-id="06adc-128">string</span></span> | <span data-ttu-id="06adc-p104">同じユーザー コレクションの前の**デルタ**関数の `deltaLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、変更追跡のその回が完了したことを示します。このコレクションについて、このトークンを含む、`deltaLink` URL 全体を次の変更追跡のラウンドの最初の要求に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="06adc-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="06adc-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="06adc-131">$skiptoken</span></span> | <span data-ttu-id="06adc-132">string</span><span class="sxs-lookup"><span data-stu-id="06adc-132">string</span></span> | <span data-ttu-id="06adc-133">前の**デルタ**関数の `nextLink` URL で[状態トークン](../../../concepts/delta_query_overview.md)が返され、同じユーザー コレクションで追跡されるその他の変更があることを示します。</span><span class="sxs-lookup"><span data-stu-id="06adc-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="06adc-134">OData クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="06adc-134">OData query parameters</span></span>

<span data-ttu-id="06adc-135">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="06adc-135">This method supports the OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="06adc-p105">任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="06adc-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="06adc-138">デルタ クエリは、メッセージの `$select`、`$top`、および `$expand` をサポートします。</span><span class="sxs-lookup"><span data-stu-id="06adc-138">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="06adc-139">と `$orderby` に対するサポートには制限があります。`$filter`</span><span class="sxs-lookup"><span data-stu-id="06adc-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="06adc-140">サポートされている唯一の`$filter` 式は、一人または二人の特定ユーザーでの変更を追跡する `$filter=id+eq+{value}` あるいは `$filter=id+eq+{value1}+or+id+eq+{value2}` です。 `$filter=id+eq+{value1}+or+id+eq+{value2}`</span><span class="sxs-lookup"><span data-stu-id="06adc-140">The only supported `$filter` expression is for tracking changes on one or two specific users:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`</span></span> 
  * <span data-ttu-id="06adc-141">サポートされている唯一の `$orderby` 式は、`$orderby=receivedDateTime+desc` です。</span><span class="sxs-lookup"><span data-stu-id="06adc-141">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`.</span></span> <span data-ttu-id="06adc-142">式を含めない場合、戻り値の順序は保証されません。`$orderby`</span><span class="sxs-lookup"><span data-stu-id="06adc-142">If you do not include  an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="06adc-143">はサポートされていません。`$search`</span><span class="sxs-lookup"><span data-stu-id="06adc-143">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06adc-144">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06adc-144">Request headers</span></span>
| <span data-ttu-id="06adc-145">名前</span><span class="sxs-lookup"><span data-stu-id="06adc-145">Name</span></span>       | <span data-ttu-id="06adc-146">説明</span><span class="sxs-lookup"><span data-stu-id="06adc-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06adc-147">承認</span><span class="sxs-lookup"><span data-stu-id="06adc-147">Authorization</span></span>  | <span data-ttu-id="06adc-148">ベアラー&lt;トークン&gt;</span><span class="sxs-lookup"><span data-stu-id="06adc-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="06adc-149">コンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="06adc-149">Content-Type</span></span>  | <span data-ttu-id="06adc-150">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="06adc-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="06adc-151">要求本文</span><span class="sxs-lookup"><span data-stu-id="06adc-151">Request body</span></span>
<span data-ttu-id="06adc-152">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="06adc-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06adc-153">応答</span><span class="sxs-lookup"><span data-stu-id="06adc-153">Response</span></span>

<span data-ttu-id="06adc-p107">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) コレクション オブジェクトを返します。応答には、nextLink URL または deltaLink URL も含まれます。</span><span class="sxs-lookup"><span data-stu-id="06adc-p107">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body. The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="06adc-p108">nextLink URL が返される場合は、セッションに取得するデータの追加ページがあります。deltaLink URL が応答で返されるまで、アプリケーションは nextLink URL を使用して要求を実行し続けます。</span><span class="sxs-lookup"><span data-stu-id="06adc-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="06adc-p109">deltaLink URL が返される場合、返されるリソースの既存の状態に関するデータはありません。以降の要求では、アプリケーションは deltaLink URL を使用して、リソースへの変更点を確認します。</span><span class="sxs-lookup"><span data-stu-id="06adc-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="06adc-160">参照先:</span><span class="sxs-lookup"><span data-stu-id="06adc-160">See:</span></span></br>
- <span data-ttu-id="06adc-161">詳細については、「[デルタ クエリの使用](../../../concepts/delta_query_overview.md)」をご覧ください</span><span class="sxs-lookup"><span data-stu-id="06adc-161">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="06adc-162">要求の例については、「[ユーザーに対する増分の変更の取得](../../../concepts/delta_query_users.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="06adc-162">[Get incremental changes for users](../../../concepts/delta_query_users.md) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="06adc-163">例</span><span class="sxs-lookup"><span data-stu-id="06adc-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06adc-164">要求</span><span class="sxs-lookup"><span data-stu-id="06adc-164">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/delta
```

##### <a name="response"></a><span data-ttu-id="06adc-165">応答</span><span class="sxs-lookup"><span data-stu-id="06adc-165">Response</span></span>
<span data-ttu-id="06adc-p110">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="06adc-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->