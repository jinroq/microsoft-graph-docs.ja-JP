# <a name="create-contact"></a><span data-ttu-id="bae3d-101">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="bae3d-101">Create Contact</span></span>

<span data-ttu-id="bae3d-102">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="bae3d-102">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="bae3d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bae3d-103">Permissions</span></span>

<span data-ttu-id="bae3d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bae3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bae3d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bae3d-106">Permission type</span></span>      | <span data-ttu-id="bae3d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bae3d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bae3d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bae3d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bae3d-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bae3d-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bae3d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bae3d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bae3d-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bae3d-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bae3d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bae3d-112">Application</span></span> | <span data-ttu-id="bae3d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bae3d-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bae3d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bae3d-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="bae3d-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bae3d-115">Request headers</span></span>

| <span data-ttu-id="bae3d-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bae3d-116">Header</span></span>       | <span data-ttu-id="bae3d-117">値</span><span class="sxs-lookup"><span data-stu-id="bae3d-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bae3d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae3d-118">Authorization</span></span>  | <span data-ttu-id="bae3d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bae3d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bae3d-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bae3d-121">Content-Type</span></span>  | <span data-ttu-id="bae3d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bae3d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bae3d-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="bae3d-124">Request body</span></span>
<span data-ttu-id="bae3d-125">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bae3d-125">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bae3d-126">応答</span><span class="sxs-lookup"><span data-stu-id="bae3d-126">Response</span></span>

<span data-ttu-id="bae3d-127">成功した場合、このメソッドは `201 Created` 応答コードと[連絡先](../resources/contact.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="bae3d-127">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bae3d-128">例</span><span class="sxs-lookup"><span data-stu-id="bae3d-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="bae3d-129">要求</span><span class="sxs-lookup"><span data-stu-id="bae3d-129">Request</span></span>

<span data-ttu-id="bae3d-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bae3d-130">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<span data-ttu-id="bae3d-131">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bae3d-131">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="bae3d-132">応答</span><span class="sxs-lookup"><span data-stu-id="bae3d-132">Response</span></span>

<span data-ttu-id="bae3d-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bae3d-133">Here is an example of the response.</span></span> <span data-ttu-id="bae3d-134">**注:**簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="bae3d-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bae3d-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bae3d-135">All default properties will be returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
