# <a name="list-contacts"></a><span data-ttu-id="d8e2f-101">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d8e2f-101">List contacts</span></span>

<span data-ttu-id="d8e2f-102">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="d8e2f-102">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8e2f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d8e2f-103">Permissions</span></span>
<span data-ttu-id="d8e2f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d8e2f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8e2f-106">Permission type</span></span>      | <span data-ttu-id="d8e2f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8e2f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8e2f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8e2f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d8e2f-109">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8e2f-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d8e2f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8e2f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8e2f-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8e2f-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d8e2f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8e2f-112">Application</span></span> | <span data-ttu-id="d8e2f-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8e2f-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8e2f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8e2f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8e2f-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d8e2f-115">Optional query parameters</span></span>
<span data-ttu-id="d8e2f-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d8e2f-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8e2f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8e2f-117">Request headers</span></span>
| <span data-ttu-id="d8e2f-118">名前</span><span class="sxs-lookup"><span data-stu-id="d8e2f-118">Name</span></span>       | <span data-ttu-id="d8e2f-119">型</span><span class="sxs-lookup"><span data-stu-id="d8e2f-119">Type</span></span> | <span data-ttu-id="d8e2f-120">説明</span><span class="sxs-lookup"><span data-stu-id="d8e2f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d8e2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8e2f-121">Authorization</span></span>  | <span data-ttu-id="d8e2f-122">string</span><span class="sxs-lookup"><span data-stu-id="d8e2f-122">string</span></span>  | <span data-ttu-id="d8e2f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d8e2f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8e2f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8e2f-125">Request body</span></span>
<span data-ttu-id="d8e2f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d8e2f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8e2f-127">応答</span><span class="sxs-lookup"><span data-stu-id="d8e2f-127">Response</span></span>

<span data-ttu-id="d8e2f-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d8e2f-128">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8e2f-129">例</span><span class="sxs-lookup"><span data-stu-id="d8e2f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8e2f-130">要求</span><span class="sxs-lookup"><span data-stu-id="d8e2f-130">Request</span></span>
<span data-ttu-id="d8e2f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8e2f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="d8e2f-132">応答</span><span class="sxs-lookup"><span data-stu-id="d8e2f-132">Response</span></span>
<span data-ttu-id="d8e2f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8e2f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
