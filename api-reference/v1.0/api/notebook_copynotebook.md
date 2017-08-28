# <a name="notebook-copynotebook"></a><span data-ttu-id="55074-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="55074-101">notebook: copyNotebook</span></span>
<span data-ttu-id="55074-p101">コピー先ドキュメント ライブラリの [ノートブック] フォルダーにノートブックをコピーします。フォルダーが存在しない場合は、そのフォルダーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="55074-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="55074-104">Copy 操作では、非同期の呼び出しパターンに従います。まず Copy 操作を呼び出し、次に結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="55074-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="55074-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="55074-105">Permissions</span></span>
<span data-ttu-id="55074-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55074-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55074-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55074-108">Permission type</span></span>      | <span data-ttu-id="55074-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="55074-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55074-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="55074-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55074-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55074-111">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="55074-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55074-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55074-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55074-113">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="55074-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55074-114">Application</span></span> | <span data-ttu-id="55074-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55074-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55074-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55074-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="55074-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55074-117">Request headers</span></span>
| <span data-ttu-id="55074-118">名前</span><span class="sxs-lookup"><span data-stu-id="55074-118">Name</span></span>       | <span data-ttu-id="55074-119">型</span><span class="sxs-lookup"><span data-stu-id="55074-119">Type</span></span> | <span data-ttu-id="55074-120">説明</span><span class="sxs-lookup"><span data-stu-id="55074-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55074-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="55074-121">Authorization</span></span>  | <span data-ttu-id="55074-122">string</span><span class="sxs-lookup"><span data-stu-id="55074-122">string</span></span>  | <span data-ttu-id="55074-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="55074-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55074-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55074-125">Content-Type</span></span> | <span data-ttu-id="55074-126">string</span><span class="sxs-lookup"><span data-stu-id="55074-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="55074-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="55074-127">Request body</span></span>
<span data-ttu-id="55074-p104">要求本文では、操作に必要なパラメーターを格納する JSON オブジェクトを指定します。パラメーターが必要ない場合は、空の要求本文を送信してもかまいません。</span><span class="sxs-lookup"><span data-stu-id="55074-p104">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="55074-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="55074-130">Parameter</span></span>    | <span data-ttu-id="55074-131">型</span><span class="sxs-lookup"><span data-stu-id="55074-131">Type</span></span>   |<span data-ttu-id="55074-132">説明</span><span class="sxs-lookup"><span data-stu-id="55074-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55074-133">groupId</span><span class="sxs-lookup"><span data-stu-id="55074-133">groupId</span></span>|<span data-ttu-id="55074-134">String</span><span class="sxs-lookup"><span data-stu-id="55074-134">String</span></span>|<span data-ttu-id="55074-p105">コピー先グループの ID。Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="55074-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="55074-137">renameAs</span><span class="sxs-lookup"><span data-stu-id="55074-137">renameAs</span></span>|<span data-ttu-id="55074-138">String</span><span class="sxs-lookup"><span data-stu-id="55074-138">String</span></span>|<span data-ttu-id="55074-p106">コピーの名前。既定値は、既存のアイテムの名前になります。</span><span class="sxs-lookup"><span data-stu-id="55074-p106">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="55074-141">応答</span><span class="sxs-lookup"><span data-stu-id="55074-141">Response</span></span>

<span data-ttu-id="55074-p107">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteOperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="55074-p107">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="55074-144">例</span><span class="sxs-lookup"><span data-stu-id="55074-144">Example</span></span>
<span data-ttu-id="55074-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="55074-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="55074-146">要求</span><span class="sxs-lookup"><span data-stu-id="55074-146">Request</span></span>
<span data-ttu-id="55074-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="55074-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="55074-148">応答</span><span class="sxs-lookup"><span data-stu-id="55074-148">Response</span></span>
<span data-ttu-id="55074-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="55074-149">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
