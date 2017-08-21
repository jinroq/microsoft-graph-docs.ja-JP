# <a name="create-mailfolder"></a><span data-ttu-id="31653-101">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="31653-101">Create MailFolder</span></span>

<span data-ttu-id="31653-102">この API を使用して、ユーザーのメールボックスのルート フォルダーに新しいメール フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="31653-102">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31653-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="31653-103">Prerequisites</span></span>
<span data-ttu-id="31653-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="31653-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="31653-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31653-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="31653-106">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31653-106">Request headers</span></span>
| <span data-ttu-id="31653-107">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31653-107">Header</span></span>       | <span data-ttu-id="31653-108">値</span><span class="sxs-lookup"><span data-stu-id="31653-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31653-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="31653-109">Authorization</span></span>  | <span data-ttu-id="31653-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="31653-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="31653-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31653-112">Content-Type</span></span>  | <span data-ttu-id="31653-113">application/json</span><span class="sxs-lookup"><span data-stu-id="31653-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31653-114">要求本文</span><span class="sxs-lookup"><span data-stu-id="31653-114">Request body</span></span>
<span data-ttu-id="31653-p102">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="31653-p102">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="31653-117">パラメーター</span><span class="sxs-lookup"><span data-stu-id="31653-117">Parameter</span></span>    | <span data-ttu-id="31653-118">型</span><span class="sxs-lookup"><span data-stu-id="31653-118">Type</span></span>   |<span data-ttu-id="31653-119">説明</span><span class="sxs-lookup"><span data-stu-id="31653-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31653-120">displayName</span><span class="sxs-lookup"><span data-stu-id="31653-120">displayName</span></span>|<span data-ttu-id="31653-121">String</span><span class="sxs-lookup"><span data-stu-id="31653-121">String</span></span>|<span data-ttu-id="31653-122">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="31653-122">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="31653-123">応答</span><span class="sxs-lookup"><span data-stu-id="31653-123">Response</span></span>

<span data-ttu-id="31653-124">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31653-124">If successful, this method returns `201, Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31653-125">例</span><span class="sxs-lookup"><span data-stu-id="31653-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31653-126">要求</span><span class="sxs-lookup"><span data-stu-id="31653-126">Request</span></span>
<span data-ttu-id="31653-127">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31653-127">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="31653-128">応答</span><span class="sxs-lookup"><span data-stu-id="31653-128">Response</span></span>
<span data-ttu-id="31653-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31653-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
