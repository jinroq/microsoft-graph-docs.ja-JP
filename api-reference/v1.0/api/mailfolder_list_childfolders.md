# <a name="list-childfolders"></a><span data-ttu-id="73bfc-101">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="73bfc-101">List childFolders</span></span>

<span data-ttu-id="73bfc-p101">指定したフォルダーの下のフォルダーのコレクションを取得します。`.../me/MailFolders` ショートカットを使用して、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="73bfc-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73bfc-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="73bfc-104">Prerequisites</span></span>
<span data-ttu-id="73bfc-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.Read、Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="73bfc-105">One of the following **scopes** is required to execute this API: *Mail.Read; Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="73bfc-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73bfc-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73bfc-107">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73bfc-107">Optional query parameters</span></span>
<span data-ttu-id="73bfc-108">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="73bfc-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="73bfc-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73bfc-109">Request headers</span></span>
| <span data-ttu-id="73bfc-110">名前</span><span class="sxs-lookup"><span data-stu-id="73bfc-110">Name</span></span>       | <span data-ttu-id="73bfc-111">型</span><span class="sxs-lookup"><span data-stu-id="73bfc-111">Type</span></span> | <span data-ttu-id="73bfc-112">説明</span><span class="sxs-lookup"><span data-stu-id="73bfc-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73bfc-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="73bfc-113">Authorization</span></span>  | <span data-ttu-id="73bfc-114">string</span><span class="sxs-lookup"><span data-stu-id="73bfc-114">string</span></span>  | <span data-ttu-id="73bfc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73bfc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73bfc-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="73bfc-117">Request body</span></span>
<span data-ttu-id="73bfc-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73bfc-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73bfc-119">応答</span><span class="sxs-lookup"><span data-stu-id="73bfc-119">Response</span></span>

<span data-ttu-id="73bfc-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="73bfc-120">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73bfc-121">例</span><span class="sxs-lookup"><span data-stu-id="73bfc-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73bfc-122">要求</span><span class="sxs-lookup"><span data-stu-id="73bfc-122">Request</span></span>
<span data-ttu-id="73bfc-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73bfc-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="73bfc-124">応答</span><span class="sxs-lookup"><span data-stu-id="73bfc-124">Response</span></span>
<span data-ttu-id="73bfc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73bfc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
