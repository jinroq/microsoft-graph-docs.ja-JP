# <a name="create-contact"></a><span data-ttu-id="e1be8-101">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="e1be8-101">Create Contact</span></span>

<span data-ttu-id="e1be8-102">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="e1be8-102">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1be8-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1be8-103">Permissions</span></span>
<span data-ttu-id="e1be8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1be8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1be8-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1be8-106">Permission type</span></span>      | <span data-ttu-id="e1be8-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1be8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1be8-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1be8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e1be8-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1be8-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e1be8-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1be8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1be8-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1be8-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e1be8-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1be8-112">Application</span></span> | <span data-ttu-id="e1be8-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1be8-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1be8-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1be8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="e1be8-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1be8-115">Request headers</span></span>
| <span data-ttu-id="e1be8-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1be8-116">Header</span></span>       | <span data-ttu-id="e1be8-117">値</span><span class="sxs-lookup"><span data-stu-id="e1be8-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1be8-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1be8-118">Authorization</span></span>  | <span data-ttu-id="e1be8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1be8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1be8-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1be8-121">Content-Type</span></span>  | <span data-ttu-id="e1be8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e1be8-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1be8-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1be8-123">Request body</span></span>
<span data-ttu-id="e1be8-124">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1be8-124">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1be8-125">応答</span><span class="sxs-lookup"><span data-stu-id="e1be8-125">Response</span></span>

<span data-ttu-id="e1be8-126">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1be8-126">If successful, this method returns `201, Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1be8-127">例</span><span class="sxs-lookup"><span data-stu-id="e1be8-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1be8-128">要求</span><span class="sxs-lookup"><span data-stu-id="e1be8-128">Request</span></span>
<span data-ttu-id="e1be8-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1be8-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
<span data-ttu-id="e1be8-130">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1be8-130">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="e1be8-131">応答</span><span class="sxs-lookup"><span data-stu-id="e1be8-131">Response</span></span>
<span data-ttu-id="e1be8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1be8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
