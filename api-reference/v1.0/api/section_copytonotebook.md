# <a name="section-copytonotebook"></a><span data-ttu-id="c2ccf-101">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="c2ccf-101">section: copyToNotebook</span></span>
<span data-ttu-id="c2ccf-102">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-102">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="c2ccf-103">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次いで結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2ccf-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="c2ccf-104">Prerequisites</span></span>
<span data-ttu-id="c2ccf-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="c2ccf-106">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ccf-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="c2ccf-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2ccf-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="c2ccf-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2ccf-108">Request headers</span></span>
| <span data-ttu-id="c2ccf-109">名前</span><span class="sxs-lookup"><span data-stu-id="c2ccf-109">Name</span></span>       | <span data-ttu-id="c2ccf-110">型</span><span class="sxs-lookup"><span data-stu-id="c2ccf-110">Type</span></span> | <span data-ttu-id="c2ccf-111">説明</span><span class="sxs-lookup"><span data-stu-id="c2ccf-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2ccf-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2ccf-112">Authorization</span></span>  | <span data-ttu-id="c2ccf-113">string</span><span class="sxs-lookup"><span data-stu-id="c2ccf-113">string</span></span>  | <span data-ttu-id="c2ccf-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2ccf-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2ccf-116">Content-Type</span></span> | <span data-ttu-id="c2ccf-117">string</span><span class="sxs-lookup"><span data-stu-id="c2ccf-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c2ccf-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2ccf-118">Request body</span></span>
<span data-ttu-id="c2ccf-119">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="c2ccf-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c2ccf-120">Parameter</span></span>    | <span data-ttu-id="c2ccf-121">型</span><span class="sxs-lookup"><span data-stu-id="c2ccf-121">Type</span></span>   |<span data-ttu-id="c2ccf-122">説明</span><span class="sxs-lookup"><span data-stu-id="c2ccf-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2ccf-123">groupId</span><span class="sxs-lookup"><span data-stu-id="c2ccf-123">groupId</span></span>|<span data-ttu-id="c2ccf-124">String</span><span class="sxs-lookup"><span data-stu-id="c2ccf-124">String</span></span>|<span data-ttu-id="c2ccf-p102">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="c2ccf-127">id</span><span class="sxs-lookup"><span data-stu-id="c2ccf-127">id</span></span>|<span data-ttu-id="c2ccf-128">String</span><span class="sxs-lookup"><span data-stu-id="c2ccf-128">String</span></span>|<span data-ttu-id="c2ccf-p103">必須。コピー先ノートブックの ID。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-p103">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="c2ccf-131">renameAs</span><span class="sxs-lookup"><span data-stu-id="c2ccf-131">renameAs</span></span>|<span data-ttu-id="c2ccf-132">String</span><span class="sxs-lookup"><span data-stu-id="c2ccf-132">String</span></span>|<span data-ttu-id="c2ccf-p104">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-p104">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="c2ccf-135">応答</span><span class="sxs-lookup"><span data-stu-id="c2ccf-135">Response</span></span>

<span data-ttu-id="c2ccf-p105">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="c2ccf-138">例</span><span class="sxs-lookup"><span data-stu-id="c2ccf-138">Example</span></span>
<span data-ttu-id="c2ccf-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2ccf-140">要求</span><span class="sxs-lookup"><span data-stu-id="c2ccf-140">Request</span></span>
<span data-ttu-id="c2ccf-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="c2ccf-142">応答</span><span class="sxs-lookup"><span data-stu-id="c2ccf-142">Response</span></span>
<span data-ttu-id="c2ccf-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c2ccf-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->