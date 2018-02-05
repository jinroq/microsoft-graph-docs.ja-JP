# <a name="message-move"></a><span data-ttu-id="8c2d6-101">メッセージ: move</span><span class="sxs-lookup"><span data-stu-id="8c2d6-101">message: move</span></span>

<span data-ttu-id="8c2d6-p101">メッセージをフォルダーに移動します。これにより、宛先フォルダーにメッセージの新しいコピーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c2d6-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c2d6-104">Permissions</span></span>
<span data-ttu-id="8c2d6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c2d6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c2d6-107">Permission type</span></span>      | <span data-ttu-id="8c2d6-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c2d6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c2d6-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c2d6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8c2d6-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c2d6-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8c2d6-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c2d6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c2d6-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c2d6-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8c2d6-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c2d6-113">Application</span></span> | <span data-ttu-id="8c2d6-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c2d6-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c2d6-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c2d6-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="8c2d6-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c2d6-116">Request headers</span></span>
| <span data-ttu-id="8c2d6-117">名前</span><span class="sxs-lookup"><span data-stu-id="8c2d6-117">Name</span></span>       | <span data-ttu-id="8c2d6-118">型</span><span class="sxs-lookup"><span data-stu-id="8c2d6-118">Type</span></span> | <span data-ttu-id="8c2d6-119">説明</span><span class="sxs-lookup"><span data-stu-id="8c2d6-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c2d6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c2d6-120">Authorization</span></span>  | <span data-ttu-id="8c2d6-121">string</span><span class="sxs-lookup"><span data-stu-id="8c2d6-121">string</span></span>  | <span data-ttu-id="8c2d6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c2d6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c2d6-124">Content-Type</span></span> | <span data-ttu-id="8c2d6-125">string</span><span class="sxs-lookup"><span data-stu-id="8c2d6-125">string</span></span>  | <span data-ttu-id="8c2d6-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c2d6-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c2d6-128">Request body</span></span>
<span data-ttu-id="8c2d6-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c2d6-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c2d6-130">Parameter</span></span>    | <span data-ttu-id="8c2d6-131">型</span><span class="sxs-lookup"><span data-stu-id="8c2d6-131">Type</span></span>   |<span data-ttu-id="8c2d6-132">説明</span><span class="sxs-lookup"><span data-stu-id="8c2d6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c2d6-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="8c2d6-133">DestinationId</span></span>|<span data-ttu-id="8c2d6-134">String</span><span class="sxs-lookup"><span data-stu-id="8c2d6-134">String</span></span>|<span data-ttu-id="8c2d6-135">宛先フォルダー ID、または *Inbox*、*Drafts*、*SentItems*、*DeletedItems* などの、既知のフォルダー名。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-135">The destination folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="8c2d6-136">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="8c2d6-137">応答</span><span class="sxs-lookup"><span data-stu-id="8c2d6-137">Response</span></span>

<span data-ttu-id="8c2d6-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-138">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c2d6-139">例</span><span class="sxs-lookup"><span data-stu-id="8c2d6-139">Example</span></span>
<span data-ttu-id="8c2d6-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c2d6-141">要求</span><span class="sxs-lookup"><span data-stu-id="8c2d6-141">Request</span></span>
<span data-ttu-id="8c2d6-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/move
Content-type: application/json
Content-length: 44

{
  "DestinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="8c2d6-143">応答</span><span class="sxs-lookup"><span data-stu-id="8c2d6-143">Response</span></span>
<span data-ttu-id="8c2d6-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c2d6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
