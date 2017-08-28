# <a name="create-contactfolder"></a><span data-ttu-id="117f8-101">ContactFolder を作成する　</span><span class="sxs-lookup"><span data-stu-id="117f8-101">Create ContactFolder</span></span>

<span data-ttu-id="117f8-102">ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="117f8-102">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="117f8-103">また、[指定した連絡先フォルダーの子として新しい contactfolder を作成](contactfolder_post_childfolders.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="117f8-103">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder_post_childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="117f8-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="117f8-104">Permissions</span></span>
<span data-ttu-id="117f8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="117f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="117f8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="117f8-107">Permission type</span></span>      | <span data-ttu-id="117f8-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="117f8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="117f8-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="117f8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="117f8-110">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="117f8-110">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="117f8-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="117f8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="117f8-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="117f8-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="117f8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="117f8-113">Application</span></span> | <span data-ttu-id="117f8-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="117f8-114">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="117f8-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="117f8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="117f8-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="117f8-116">Request headers</span></span>
| <span data-ttu-id="117f8-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="117f8-117">Header</span></span>       | <span data-ttu-id="117f8-118">値</span><span class="sxs-lookup"><span data-stu-id="117f8-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="117f8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="117f8-119">Authorization</span></span>  | <span data-ttu-id="117f8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="117f8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="117f8-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="117f8-122">Content-Type</span></span>  | <span data-ttu-id="117f8-123">application/json</span><span class="sxs-lookup"><span data-stu-id="117f8-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="117f8-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="117f8-124">Request body</span></span>
<span data-ttu-id="117f8-125">要求本文で、[ContactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="117f8-125">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="117f8-126">応答</span><span class="sxs-lookup"><span data-stu-id="117f8-126">Response</span></span>

<span data-ttu-id="117f8-127">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [ContactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="117f8-127">If successful, this method returns `201, Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="117f8-128">例</span><span class="sxs-lookup"><span data-stu-id="117f8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="117f8-129">要求</span><span class="sxs-lookup"><span data-stu-id="117f8-129">Request</span></span>
<span data-ttu-id="117f8-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="117f8-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="117f8-131">要求本文で、[contactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="117f8-131">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="117f8-132">応答</span><span class="sxs-lookup"><span data-stu-id="117f8-132">Response</span></span>
<span data-ttu-id="117f8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="117f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
