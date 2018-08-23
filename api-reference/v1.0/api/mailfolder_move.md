# <a name="mailfolder-move"></a><span data-ttu-id="5ed6e-101">mailFolder: 移動</span><span class="sxs-lookup"><span data-stu-id="5ed6e-101">mailFolder: move</span></span>

<span data-ttu-id="5ed6e-102">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ed6e-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ed6e-103">Permissions</span></span>

<span data-ttu-id="5ed6e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="5ed6e-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ed6e-106">Permission type</span></span> | <span data-ttu-id="5ed6e-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ed6e-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="5ed6e-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ed6e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5ed6e-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ed6e-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5ed6e-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ed6e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ed6e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ed6e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5ed6e-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ed6e-112">Application</span></span> | <span data-ttu-id="5ed6e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ed6e-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ed6e-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ed6e-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="5ed6e-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ed6e-115">Request headers</span></span>

| <span data-ttu-id="5ed6e-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ed6e-116">Header</span></span> | <span data-ttu-id="5ed6e-117">値</span><span class="sxs-lookup"><span data-stu-id="5ed6e-117">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="5ed6e-118">承認</span><span class="sxs-lookup"><span data-stu-id="5ed6e-118">Authorization</span></span> | <span data-ttu-id="5ed6e-119">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="5ed6e-119"></span></span> <span data-ttu-id="5ed6e-120">必須です。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-120">Required.</span></span> |
| <span data-ttu-id="5ed6e-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ed6e-121">Content-Type</span></span> | <span data-ttu-id="5ed6e-122">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="5ed6e-122"></span></span> <span data-ttu-id="5ed6e-123">必須です。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ed6e-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ed6e-124">Request body</span></span>

<span data-ttu-id="5ed6e-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5ed6e-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ed6e-126">Parameter</span></span> | <span data-ttu-id="5ed6e-127">型</span><span class="sxs-lookup"><span data-stu-id="5ed6e-127">Type</span></span> | <span data-ttu-id="5ed6e-128">説明</span><span class="sxs-lookup"><span data-stu-id="5ed6e-128">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="5ed6e-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="5ed6e-129">destinationId</span></span>|<span data-ttu-id="5ed6e-130">文字列</span><span class="sxs-lookup"><span data-stu-id="5ed6e-130">String</span></span>|<span data-ttu-id="5ed6e-131">フォルダー ID または既知のフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-131">The folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="5ed6e-132">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="5ed6e-133">応答</span><span class="sxs-lookup"><span data-stu-id="5ed6e-133">Response</span></span>

<span data-ttu-id="5ed6e-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文の [mailFolder](../resources/mailfolder.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ed6e-135">例</span><span class="sxs-lookup"><span data-stu-id="5ed6e-135">Example</span></span>

<span data-ttu-id="5ed6e-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-136">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5ed6e-137">要求</span><span class="sxs-lookup"><span data-stu-id="5ed6e-137">Request</span></span>

<span data-ttu-id="5ed6e-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5ed6e-139">応答</span><span class="sxs-lookup"><span data-stu-id="5ed6e-139">Response</span></span>

<span data-ttu-id="5ed6e-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-140">Here is an example of the response.</span></span>

> <span data-ttu-id="5ed6e-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ed6e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
