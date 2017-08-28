# <a name="get-message"></a><span data-ttu-id="706a9-101">メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="706a9-101">Get message</span></span>

<span data-ttu-id="706a9-102">[メッセージ](../resources/message.md) オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="706a9-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="706a9-103">**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`GET` 操作を使用して、**メッセージ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="706a9-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="706a9-104">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="706a9-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="706a9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="706a9-105">Permissions</span></span>
<span data-ttu-id="706a9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="706a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="706a9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="706a9-108">Permission type</span></span>      | <span data-ttu-id="706a9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="706a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="706a9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="706a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="706a9-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="706a9-111">Mail.Read</span></span>    |
|<span data-ttu-id="706a9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="706a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="706a9-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="706a9-113">Mail.Read</span></span>    |
|<span data-ttu-id="706a9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="706a9-114">Application</span></span> | <span data-ttu-id="706a9-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="706a9-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="706a9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="706a9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="706a9-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="706a9-117">Optional query parameters</span></span>
<span data-ttu-id="706a9-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="706a9-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="706a9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="706a9-119">Request headers</span></span>
| <span data-ttu-id="706a9-120">名前</span><span class="sxs-lookup"><span data-stu-id="706a9-120">Name</span></span>       | <span data-ttu-id="706a9-121">型</span><span class="sxs-lookup"><span data-stu-id="706a9-121">Type</span></span> | <span data-ttu-id="706a9-122">説明</span><span class="sxs-lookup"><span data-stu-id="706a9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="706a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="706a9-123">Authorization</span></span>  | <span data-ttu-id="706a9-124">string</span><span class="sxs-lookup"><span data-stu-id="706a9-124">string</span></span>  | <span data-ttu-id="706a9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="706a9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="706a9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="706a9-127">Request body</span></span>
<span data-ttu-id="706a9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="706a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="706a9-129">応答</span><span class="sxs-lookup"><span data-stu-id="706a9-129">Response</span></span>

<span data-ttu-id="706a9-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="706a9-130">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="706a9-131">例</span><span class="sxs-lookup"><span data-stu-id="706a9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="706a9-132">要求</span><span class="sxs-lookup"><span data-stu-id="706a9-132">Request</span></span>
<span data-ttu-id="706a9-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="706a9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="706a9-134">応答</span><span class="sxs-lookup"><span data-stu-id="706a9-134">Response</span></span>
<span data-ttu-id="706a9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="706a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="706a9-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="706a9-138">See also</span></span>

- [<span data-ttu-id="706a9-139">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="706a9-139">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="706a9-140">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="706a9-140">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
