# <a name="page-copytosection"></a><span data-ttu-id="c2891-101">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="c2891-101">page: copyToSection</span></span>
<span data-ttu-id="c2891-102">特定のセクションにページをコピーします。</span><span class="sxs-lookup"><span data-stu-id="c2891-102">Copies a page to a specific section.</span></span>

<span data-ttu-id="c2891-103">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="c2891-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2891-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c2891-104">Permissions</span></span>
<span data-ttu-id="c2891-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2891-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c2891-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2891-107">Permission type</span></span>      | <span data-ttu-id="c2891-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2891-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2891-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2891-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c2891-110">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2891-110">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2891-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2891-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2891-112">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2891-112">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2891-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2891-113">Application</span></span> | <span data-ttu-id="c2891-114">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2891-114">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2891-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2891-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="c2891-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2891-116">Request headers</span></span>
| <span data-ttu-id="c2891-117">名前</span><span class="sxs-lookup"><span data-stu-id="c2891-117">Name</span></span>       | <span data-ttu-id="c2891-118">型</span><span class="sxs-lookup"><span data-stu-id="c2891-118">Type</span></span> | <span data-ttu-id="c2891-119">説明</span><span class="sxs-lookup"><span data-stu-id="c2891-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2891-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2891-120">Authorization</span></span>  | <span data-ttu-id="c2891-121">string</span><span class="sxs-lookup"><span data-stu-id="c2891-121">string</span></span>  | <span data-ttu-id="c2891-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c2891-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2891-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2891-124">Content-Type</span></span> | <span data-ttu-id="c2891-125">string</span><span class="sxs-lookup"><span data-stu-id="c2891-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c2891-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2891-126">Request body</span></span>
<span data-ttu-id="c2891-127">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c2891-127">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="c2891-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c2891-128">Parameter</span></span>    | <span data-ttu-id="c2891-129">型</span><span class="sxs-lookup"><span data-stu-id="c2891-129">Type</span></span>   |<span data-ttu-id="c2891-130">説明</span><span class="sxs-lookup"><span data-stu-id="c2891-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2891-131">groupId</span><span class="sxs-lookup"><span data-stu-id="c2891-131">groupId</span></span>|<span data-ttu-id="c2891-132">String</span><span class="sxs-lookup"><span data-stu-id="c2891-132">String</span></span>|<span data-ttu-id="c2891-p103">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="c2891-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="c2891-135">id</span><span class="sxs-lookup"><span data-stu-id="c2891-135">id</span></span>|<span data-ttu-id="c2891-136">String</span><span class="sxs-lookup"><span data-stu-id="c2891-136">String</span></span>|<span data-ttu-id="c2891-p104">必須。コピー先セクションの ID です。</span><span class="sxs-lookup"><span data-stu-id="c2891-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="c2891-139">応答</span><span class="sxs-lookup"><span data-stu-id="c2891-139">Response</span></span>

<span data-ttu-id="c2891-p105">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="c2891-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="c2891-142">例</span><span class="sxs-lookup"><span data-stu-id="c2891-142">Example</span></span>
<span data-ttu-id="c2891-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c2891-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2891-144">要求</span><span class="sxs-lookup"><span data-stu-id="c2891-144">Request</span></span>
<span data-ttu-id="c2891-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2891-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="c2891-146">応答</span><span class="sxs-lookup"><span data-stu-id="c2891-146">Response</span></span>
<span data-ttu-id="c2891-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c2891-147">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->