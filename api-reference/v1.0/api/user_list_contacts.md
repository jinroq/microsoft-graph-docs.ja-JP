# <a name="list-contacts"></a><span data-ttu-id="2a7ec-101">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2a7ec-101">List contacts</span></span>

<span data-ttu-id="2a7ec-102">サインイン中のユーザーの既定の連絡先フォルダーから連絡先コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2a7ec-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a7ec-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="2a7ec-103">Prerequisites</span></span>
<span data-ttu-id="2a7ec-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Contacts.Read、Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="2a7ec-104">One of the following **scopes** is required to execute this API: *Contacts.Read; Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="2a7ec-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a7ec-105">HTTP request</span></span>

<span data-ttu-id="2a7ec-106">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="2a7ec-106">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="2a7ec-107">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="2a7ec-107">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2a7ec-108">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a7ec-108">Optional query parameters</span></span>
<span data-ttu-id="2a7ec-109">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2a7ec-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2a7ec-110">たとえば、`$filter` クエリ パラメーターを使って、メール アドレスのドメインに基づいて連絡先をフィルターすることができます。</span><span class="sxs-lookup"><span data-stu-id="2a7ec-110">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="2a7ec-111">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a7ec-111">Request headers</span></span>
| <span data-ttu-id="2a7ec-112">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a7ec-112">Header</span></span>       | <span data-ttu-id="2a7ec-113">値</span><span class="sxs-lookup"><span data-stu-id="2a7ec-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a7ec-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a7ec-114">Authorization</span></span>  | <span data-ttu-id="2a7ec-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a7ec-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2a7ec-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a7ec-117">Content-Type</span></span>   | <span data-ttu-id="2a7ec-118">application/json</span><span class="sxs-lookup"><span data-stu-id="2a7ec-118">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="2a7ec-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a7ec-119">Request body</span></span>
<span data-ttu-id="2a7ec-120">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a7ec-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a7ec-121">応答</span><span class="sxs-lookup"><span data-stu-id="2a7ec-121">Response</span></span>

<span data-ttu-id="2a7ec-122">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2a7ec-122">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2a7ec-123">例</span><span class="sxs-lookup"><span data-stu-id="2a7ec-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a7ec-124">要求</span><span class="sxs-lookup"><span data-stu-id="2a7ec-124">Request</span></span>
<span data-ttu-id="2a7ec-125">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a7ec-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="2a7ec-126">応答</span><span class="sxs-lookup"><span data-stu-id="2a7ec-126">Response</span></span>
<span data-ttu-id="2a7ec-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a7ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
