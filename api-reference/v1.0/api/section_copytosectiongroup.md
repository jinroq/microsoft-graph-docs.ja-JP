# <a name="section-copytosectiongroup"></a><span data-ttu-id="4db2c-101">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="4db2c-101">section: copyToSectionGroup</span></span>
<span data-ttu-id="4db2c-102">特定のセクション グループにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="4db2c-102">Copies a section to a specific section group.</span></span>

<span data-ttu-id="4db2c-103">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次いで結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="4db2c-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4db2c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="4db2c-104">Prerequisites</span></span>
<span data-ttu-id="4db2c-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="4db2c-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="4db2c-106">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db2c-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="4db2c-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4db2c-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="4db2c-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4db2c-108">Request headers</span></span>
| <span data-ttu-id="4db2c-109">名前</span><span class="sxs-lookup"><span data-stu-id="4db2c-109">Name</span></span>       | <span data-ttu-id="4db2c-110">型</span><span class="sxs-lookup"><span data-stu-id="4db2c-110">Type</span></span> | <span data-ttu-id="4db2c-111">説明</span><span class="sxs-lookup"><span data-stu-id="4db2c-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4db2c-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="4db2c-112">Authorization</span></span>  | <span data-ttu-id="4db2c-113">string</span><span class="sxs-lookup"><span data-stu-id="4db2c-113">string</span></span>  | <span data-ttu-id="4db2c-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4db2c-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4db2c-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4db2c-116">Content-Type</span></span> | <span data-ttu-id="4db2c-117">string</span><span class="sxs-lookup"><span data-stu-id="4db2c-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4db2c-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="4db2c-118">Request body</span></span>
<span data-ttu-id="4db2c-119">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4db2c-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="4db2c-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4db2c-120">Parameter</span></span>    | <span data-ttu-id="4db2c-121">型</span><span class="sxs-lookup"><span data-stu-id="4db2c-121">Type</span></span>   |<span data-ttu-id="4db2c-122">説明</span><span class="sxs-lookup"><span data-stu-id="4db2c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4db2c-123">groupId</span><span class="sxs-lookup"><span data-stu-id="4db2c-123">groupId</span></span>|<span data-ttu-id="4db2c-124">String</span><span class="sxs-lookup"><span data-stu-id="4db2c-124">String</span></span>|<span data-ttu-id="4db2c-p102">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="4db2c-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="4db2c-127">id</span><span class="sxs-lookup"><span data-stu-id="4db2c-127">id</span></span>|<span data-ttu-id="4db2c-128">String</span><span class="sxs-lookup"><span data-stu-id="4db2c-128">String</span></span>|<span data-ttu-id="4db2c-p103">必須。目的のセクション グループの ID。</span><span class="sxs-lookup"><span data-stu-id="4db2c-p103">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="4db2c-131">renameAs</span><span class="sxs-lookup"><span data-stu-id="4db2c-131">renameAs</span></span>|<span data-ttu-id="4db2c-132">String</span><span class="sxs-lookup"><span data-stu-id="4db2c-132">String</span></span>|<span data-ttu-id="4db2c-p104">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="4db2c-p104">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="4db2c-135">応答</span><span class="sxs-lookup"><span data-stu-id="4db2c-135">Response</span></span>

<span data-ttu-id="4db2c-p105">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="4db2c-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4db2c-138">例</span><span class="sxs-lookup"><span data-stu-id="4db2c-138">Example</span></span>
<span data-ttu-id="4db2c-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4db2c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4db2c-140">要求</span><span class="sxs-lookup"><span data-stu-id="4db2c-140">Request</span></span>
<span data-ttu-id="4db2c-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4db2c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="4db2c-142">応答</span><span class="sxs-lookup"><span data-stu-id="4db2c-142">Response</span></span>
<span data-ttu-id="4db2c-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4db2c-143">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->