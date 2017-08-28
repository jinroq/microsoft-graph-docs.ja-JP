# <a name="create-mailfolder"></a><span data-ttu-id="d144a-101">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="d144a-101">Create MailFolder</span></span>

<span data-ttu-id="d144a-102">この API を使用して、ユーザーのメールボックスのルート フォルダーに新しいメール フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="d144a-102">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="d144a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d144a-103">Permissions</span></span>
<span data-ttu-id="d144a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d144a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d144a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d144a-106">Permission type</span></span>      | <span data-ttu-id="d144a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d144a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d144a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d144a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d144a-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d144a-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d144a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d144a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d144a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d144a-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d144a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d144a-112">Application</span></span> | <span data-ttu-id="d144a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d144a-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d144a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d144a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="d144a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d144a-115">Request headers</span></span>
| <span data-ttu-id="d144a-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d144a-116">Header</span></span>       | <span data-ttu-id="d144a-117">値</span><span class="sxs-lookup"><span data-stu-id="d144a-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d144a-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d144a-118">Authorization</span></span>  | <span data-ttu-id="d144a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d144a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d144a-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d144a-121">Content-Type</span></span>  | <span data-ttu-id="d144a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d144a-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d144a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d144a-123">Request body</span></span>
<span data-ttu-id="d144a-p103">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="d144a-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="d144a-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d144a-126">Parameter</span></span>    | <span data-ttu-id="d144a-127">型</span><span class="sxs-lookup"><span data-stu-id="d144a-127">Type</span></span>   |<span data-ttu-id="d144a-128">説明</span><span class="sxs-lookup"><span data-stu-id="d144a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d144a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d144a-129">displayName</span></span>|<span data-ttu-id="d144a-130">String</span><span class="sxs-lookup"><span data-stu-id="d144a-130">String</span></span>|<span data-ttu-id="d144a-131">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="d144a-131">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="d144a-132">応答</span><span class="sxs-lookup"><span data-stu-id="d144a-132">Response</span></span>

<span data-ttu-id="d144a-133">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d144a-133">If successful, this method returns `201, Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d144a-134">例</span><span class="sxs-lookup"><span data-stu-id="d144a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d144a-135">要求</span><span class="sxs-lookup"><span data-stu-id="d144a-135">Request</span></span>
<span data-ttu-id="d144a-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d144a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="d144a-137">応答</span><span class="sxs-lookup"><span data-stu-id="d144a-137">Response</span></span>
<span data-ttu-id="d144a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d144a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
