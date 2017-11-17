# <a name="message-copy"></a><span data-ttu-id="13a2b-101">メッセージ: copy</span><span class="sxs-lookup"><span data-stu-id="13a2b-101">message: copy</span></span>

<span data-ttu-id="13a2b-102">メッセージをフォルダーにコピーします。</span><span class="sxs-lookup"><span data-stu-id="13a2b-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="13a2b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13a2b-103">Permissions</span></span>
<span data-ttu-id="13a2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13a2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="13a2b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13a2b-106">Permission type</span></span>      | <span data-ttu-id="13a2b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="13a2b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13a2b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13a2b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="13a2b-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13a2b-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13a2b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13a2b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13a2b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13a2b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13a2b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13a2b-112">Application</span></span> | <span data-ttu-id="13a2b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13a2b-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="13a2b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13a2b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```
## <a name="request-headers"></a><span data-ttu-id="13a2b-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13a2b-115">Request headers</span></span>
| <span data-ttu-id="13a2b-116">名前</span><span class="sxs-lookup"><span data-stu-id="13a2b-116">Name</span></span>       | <span data-ttu-id="13a2b-117">型</span><span class="sxs-lookup"><span data-stu-id="13a2b-117">Type</span></span> | <span data-ttu-id="13a2b-118">説明</span><span class="sxs-lookup"><span data-stu-id="13a2b-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="13a2b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="13a2b-119">Authorization</span></span>  | <span data-ttu-id="13a2b-120">string</span><span class="sxs-lookup"><span data-stu-id="13a2b-120">string</span></span>  | <span data-ttu-id="13a2b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="13a2b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13a2b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13a2b-123">Content-Type</span></span> | <span data-ttu-id="13a2b-124">string</span><span class="sxs-lookup"><span data-stu-id="13a2b-124">string</span></span>  | <span data-ttu-id="13a2b-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="13a2b-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13a2b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="13a2b-127">Request body</span></span>
<span data-ttu-id="13a2b-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="13a2b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="13a2b-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="13a2b-129">Parameter</span></span>    | <span data-ttu-id="13a2b-130">型</span><span class="sxs-lookup"><span data-stu-id="13a2b-130">Type</span></span>   |<span data-ttu-id="13a2b-131">説明</span><span class="sxs-lookup"><span data-stu-id="13a2b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13a2b-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="13a2b-132">destinationId</span></span>|<span data-ttu-id="13a2b-133">String</span><span class="sxs-lookup"><span data-stu-id="13a2b-133">String</span></span>|<span data-ttu-id="13a2b-134">宛先フォルダーの ID、あるいは `Inbox`、`Drafts`、`SentItems` または `DeletedItems` の既知のフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="13a2b-134">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="13a2b-135">応答</span><span class="sxs-lookup"><span data-stu-id="13a2b-135">Response</span></span>

<span data-ttu-id="13a2b-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="13a2b-136">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a2b-137">例</span><span class="sxs-lookup"><span data-stu-id="13a2b-137">Example</span></span>
<span data-ttu-id="13a2b-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="13a2b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="13a2b-139">要求</span><span class="sxs-lookup"><span data-stu-id="13a2b-139">Request</span></span>
<span data-ttu-id="13a2b-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13a2b-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="13a2b-141">応答</span><span class="sxs-lookup"><span data-stu-id="13a2b-141">Response</span></span>
<span data-ttu-id="13a2b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13a2b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
