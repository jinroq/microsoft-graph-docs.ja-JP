# <a name="mailfolder-move"></a><span data-ttu-id="aff46-101">mailFolder: 移動</span><span class="sxs-lookup"><span data-stu-id="aff46-101">mailFolder: move</span></span>

<span data-ttu-id="aff46-102">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="aff46-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="aff46-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aff46-103">Permissions</span></span>
<span data-ttu-id="aff46-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aff46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aff46-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aff46-106">Permission type</span></span>      | <span data-ttu-id="aff46-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aff46-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aff46-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aff46-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aff46-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aff46-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aff46-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aff46-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aff46-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aff46-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aff46-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aff46-112">Application</span></span> | <span data-ttu-id="aff46-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aff46-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aff46-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aff46-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="aff46-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aff46-115">Request headers</span></span>
| <span data-ttu-id="aff46-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aff46-116">Header</span></span>       | <span data-ttu-id="aff46-117">値</span><span class="sxs-lookup"><span data-stu-id="aff46-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aff46-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="aff46-118">Authorization</span></span>  | <span data-ttu-id="aff46-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aff46-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aff46-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aff46-121">Content-Type</span></span>  | <span data-ttu-id="aff46-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="aff46-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aff46-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="aff46-124">Request body</span></span>
<span data-ttu-id="aff46-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="aff46-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aff46-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="aff46-126">Parameter</span></span>    | <span data-ttu-id="aff46-127">型</span><span class="sxs-lookup"><span data-stu-id="aff46-127">Type</span></span>   |<span data-ttu-id="aff46-128">説明</span><span class="sxs-lookup"><span data-stu-id="aff46-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aff46-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="aff46-129">destinationId</span></span>|<span data-ttu-id="aff46-130">String</span><span class="sxs-lookup"><span data-stu-id="aff46-130">String</span></span>|<span data-ttu-id="aff46-131">フォルダー ID、または *Inbox*、*Drafts*、*SentItems*、*DeletedItems* などの、既知のフォルダー名。</span><span class="sxs-lookup"><span data-stu-id="aff46-131">The folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="aff46-132">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aff46-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="aff46-133">応答</span><span class="sxs-lookup"><span data-stu-id="aff46-133">Response</span></span>

<span data-ttu-id="aff46-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aff46-134">If successful, this method returns `200 OK` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aff46-135">例</span><span class="sxs-lookup"><span data-stu-id="aff46-135">Example</span></span>
<span data-ttu-id="aff46-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="aff46-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aff46-137">要求</span><span class="sxs-lookup"><span data-stu-id="aff46-137">Request</span></span>
<span data-ttu-id="aff46-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aff46-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="aff46-139">応答</span><span class="sxs-lookup"><span data-stu-id="aff46-139">Response</span></span>
<span data-ttu-id="aff46-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aff46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
