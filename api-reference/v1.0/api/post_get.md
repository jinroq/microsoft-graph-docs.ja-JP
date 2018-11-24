# <a name="get-post"></a><span data-ttu-id="79698-101">投稿を取得する</span><span class="sxs-lookup"><span data-stu-id="79698-101">Get post</span></span>

<span data-ttu-id="79698-p101">指定したスレッド内の投稿のプロパティと関係を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="79698-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="79698-104">**投稿**リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`GET` 操作を使用して、**投稿**インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="79698-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="79698-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79698-105">Permissions</span></span>
<span data-ttu-id="79698-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79698-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79698-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79698-108">Permission type</span></span>      | <span data-ttu-id="79698-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79698-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79698-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79698-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79698-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79698-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="79698-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79698-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79698-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79698-113">Not supported.</span></span>    |
|<span data-ttu-id="79698-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79698-114">Application</span></span> | <span data-ttu-id="79698-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79698-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79698-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79698-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79698-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79698-117">Optional query parameters</span></span>
<span data-ttu-id="79698-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79698-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="79698-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79698-119">Request headers</span></span>
| <span data-ttu-id="79698-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79698-120">Header</span></span>       | <span data-ttu-id="79698-121">値</span><span class="sxs-lookup"><span data-stu-id="79698-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79698-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79698-122">Authorization</span></span>  | <span data-ttu-id="79698-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="79698-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79698-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="79698-125">Request body</span></span>
<span data-ttu-id="79698-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79698-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79698-127">応答</span><span class="sxs-lookup"><span data-stu-id="79698-127">Response</span></span>

<span data-ttu-id="79698-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[投稿](../resources/post.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79698-128">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79698-129">例</span><span class="sxs-lookup"><span data-stu-id="79698-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79698-130">要求</span><span class="sxs-lookup"><span data-stu-id="79698-130">Request</span></span>
<span data-ttu-id="79698-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79698-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="79698-132">応答</span><span class="sxs-lookup"><span data-stu-id="79698-132">Response</span></span>
<span data-ttu-id="79698-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79698-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

{
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "receivedDateTime": "datetime-value",
  "hasAttachments": true,
  "from": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  },
  "sender": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="79698-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="79698-136">See also</span></span>

- [<span data-ttu-id="79698-137">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="79698-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="79698-138">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="79698-138">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
