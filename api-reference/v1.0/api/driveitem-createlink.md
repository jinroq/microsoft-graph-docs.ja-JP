---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルをリンクで共有する
localization_priority: Normal
ms.prod: sharepoint
description: createLink アクションを使用して、共有リンクを使って DriveItem を共有できます。
doc_type: apiPageType
ms.openlocfilehash: ebb13629e4e329c6e473dcf700fba58a59d8e8dc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015566"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="c807a-103">DriveItem の共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="c807a-103">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="c807a-104">**createLink** アクションを使用して、共有リンクを使って [DriveItem](../resources/driveitem.md) を共有できます。</span><span class="sxs-lookup"><span data-stu-id="c807a-104">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="c807a-p101">**createLink** アクションは、呼び出し元のアプリケーションに指定されたリンクの種類が存在しない場合に、新しい共有リンクを作成します。指定された種類の共有リンクがアプリで既に存在している場合、既存の共有リンクが返されます。</span><span class="sxs-lookup"><span data-stu-id="c807a-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="c807a-107">DriveItem リソースは、そのリソースの先祖から共有アクセス許可を継承します。</span><span class="sxs-lookup"><span data-stu-id="c807a-107">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="c807a-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c807a-108">Permissions</span></span>

<span data-ttu-id="c807a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c807a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c807a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c807a-111">Permission type</span></span>      | <span data-ttu-id="c807a-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c807a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c807a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c807a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c807a-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c807a-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c807a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c807a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c807a-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c807a-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c807a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c807a-117">Application</span></span> | <span data-ttu-id="c807a-118">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c807a-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c807a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c807a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="c807a-120">要求本文</span><span class="sxs-lookup"><span data-stu-id="c807a-120">Request body</span></span>

<span data-ttu-id="c807a-121">要求本文はアプリケーションが要求する共有リンクのプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="c807a-121">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="c807a-122">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="c807a-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="c807a-123">名前</span><span class="sxs-lookup"><span data-stu-id="c807a-123">Name</span></span>    |  <span data-ttu-id="c807a-124">種類</span><span class="sxs-lookup"><span data-stu-id="c807a-124">Type</span></span>  |                                 <span data-ttu-id="c807a-125">説明</span><span class="sxs-lookup"><span data-stu-id="c807a-125">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="c807a-126">**type**</span><span class="sxs-lookup"><span data-stu-id="c807a-126">**type**</span></span>  | <span data-ttu-id="c807a-127">string</span><span class="sxs-lookup"><span data-stu-id="c807a-127">string</span></span> | <span data-ttu-id="c807a-p104">作成する共有リンクの種類。`view`、`edit`、または `embed` です。</span><span class="sxs-lookup"><span data-stu-id="c807a-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="c807a-130">**scope**</span><span class="sxs-lookup"><span data-stu-id="c807a-130">**scope**</span></span> | <span data-ttu-id="c807a-131">string</span><span class="sxs-lookup"><span data-stu-id="c807a-131">string</span></span> | <span data-ttu-id="c807a-132">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c807a-132">Optional.</span></span> <span data-ttu-id="c807a-133">作成するリンクのスコープ。</span><span class="sxs-lookup"><span data-stu-id="c807a-133">The scope of link to create.</span></span> <span data-ttu-id="c807a-134">`anonymous` または `organization` のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="c807a-134">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="c807a-135">リンクの種類</span><span class="sxs-lookup"><span data-stu-id="c807a-135">Link types</span></span>

<span data-ttu-id="c807a-136">**type** パラメーターには次の値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="c807a-136">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="c807a-137">種類の値</span><span class="sxs-lookup"><span data-stu-id="c807a-137">Type value</span></span> | <span data-ttu-id="c807a-138">説明</span><span class="sxs-lookup"><span data-stu-id="c807a-138">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="c807a-139">その DriveItem への読み取り専用リンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="c807a-139">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="c807a-140">その DriveItem への読み取り/書き込みリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="c807a-140">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="c807a-141">その DriveItem への埋め込み可能なリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="c807a-141">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="c807a-142">このオプションは OneDrive 個人用のファイルでのみ選択可能です。</span><span class="sxs-lookup"><span data-stu-id="c807a-142">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="c807a-143">スコープの種類</span><span class="sxs-lookup"><span data-stu-id="c807a-143">Scope types</span></span>

<span data-ttu-id="c807a-144">**scope** パラメーターには次の値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="c807a-144">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="c807a-145">**scope** パラメーターが指定されていない場合、組織の既定のリンクの種類が作成されます。</span><span class="sxs-lookup"><span data-stu-id="c807a-145">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="c807a-146">値</span><span class="sxs-lookup"><span data-stu-id="c807a-146">Value</span></span>          | <span data-ttu-id="c807a-147">説明</span><span class="sxs-lookup"><span data-stu-id="c807a-147">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="c807a-148">リンクを持つすべてのユーザーが、サインインを必要とせずにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="c807a-148">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="c807a-149">これには、組織外のユーザーが含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="c807a-149">This may include people outside of your organization.</span></span> <span data-ttu-id="c807a-150">匿名リンクのサポートは、管理者によって無効にされている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c807a-150">Anonymous link support may be disabled by an administrator.</span></span>
| `organization` | <span data-ttu-id="c807a-151">組織 (テナント) にサインインしているユーザーは、リンクを使用してアクセス権を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="c807a-151">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="c807a-152">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="c807a-152">Only available in OneDrive for Business and SharePoint.</span></span>


## <a name="response"></a><span data-ttu-id="c807a-153">応答</span><span class="sxs-lookup"><span data-stu-id="c807a-153">Response</span></span>

<span data-ttu-id="c807a-154">正常に実行されると、このメソッドは要求された共有アクセス許可を表す応答本文で、単一の[アクセス許可](../resources/permission.md)リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="c807a-154">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="c807a-155">応答は、アイテムに新しい共有リンクが作成される場合は `201 Created`、既存のリンクが返される場合は `200 OK` となります。</span><span class="sxs-lookup"><span data-stu-id="c807a-155">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="c807a-156">例</span><span class="sxs-lookup"><span data-stu-id="c807a-156">Example</span></span>

<span data-ttu-id="c807a-157">次の例では、ユーザーの OneDrive の {itemId} で指定された DriveItem に対して共有リンクを作成することを要求します。</span><span class="sxs-lookup"><span data-stu-id="c807a-157">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="c807a-158">共有リンクは、読み取り専用でそのリンクによってだれでも使用可能になるよう構成されます。</span><span class="sxs-lookup"><span data-stu-id="c807a-158">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="c807a-159">要求</span><span class="sxs-lookup"><span data-stu-id="c807a-159">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c807a-160">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c807a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-link"
}-->

```http
POST /me/drive/items/{item-id}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c807a-161">C#</span><span class="sxs-lookup"><span data-stu-id="c807a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c807a-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="c807a-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c807a-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="c807a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c807a-164">Java</span><span class="sxs-lookup"><span data-stu-id="c807a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c807a-165">応答</span><span class="sxs-lookup"><span data-stu-id="c807a-165">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="c807a-166">会社の共有可能リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="c807a-166">Creating company sharable links</span></span>

<span data-ttu-id="c807a-167">OneDrive for Business および SharePoint は、会社の共有可能リンクをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="c807a-167">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="c807a-168">これらは匿名リンクに似ていますが、所有組織のメンバーだけが使用できる点が異なります。</span><span class="sxs-lookup"><span data-stu-id="c807a-168">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="c807a-169">会社の共有可能リンクを作成するには、**scope** パラメーターで値 `organization` を指定して使用します。</span><span class="sxs-lookup"><span data-stu-id="c807a-169">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="c807a-170">要求</span><span class="sxs-lookup"><span data-stu-id="c807a-170">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c807a-171">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c807a-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite", "tags": "service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c807a-172">C#</span><span class="sxs-lookup"><span data-stu-id="c807a-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c807a-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="c807a-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c807a-174">目的-C</span><span class="sxs-lookup"><span data-stu-id="c807a-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c807a-175">Java</span><span class="sxs-lookup"><span data-stu-id="c807a-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c807a-176">応答</span><span class="sxs-lookup"><span data-stu-id="c807a-176">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-embeddable-links"></a><span data-ttu-id="c807a-177">埋め込み可能なリンクを作成する</span><span class="sxs-lookup"><span data-stu-id="c807a-177">Creating embeddable links</span></span>

<span data-ttu-id="c807a-p112">リンクの種類で `embed` を使用する場合、返される webUrl は `<iframe>` HTML 要素に埋め込むことができます。埋め込みリンクが作成されると、`webHtml` プロパティに `<iframe>` がコンテンツをホストするための HTML コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c807a-p112">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="c807a-180">**注:** 埋め込みリンクは、OneDrive 個人用でのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="c807a-180">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="c807a-181">要求</span><span class="sxs-lookup"><span data-stu-id="c807a-181">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c807a-182">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c807a-182">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite", "tags": "service.onedrive service.graph" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c807a-183">C#</span><span class="sxs-lookup"><span data-stu-id="c807a-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c807a-184">Javascript</span><span class="sxs-lookup"><span data-stu-id="c807a-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c807a-185">目的-C</span><span class="sxs-lookup"><span data-stu-id="c807a-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c807a-186">Java</span><span class="sxs-lookup"><span data-stu-id="c807a-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c807a-187">応答</span><span class="sxs-lookup"><span data-stu-id="c807a-187">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedrive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="c807a-188">注釈</span><span class="sxs-lookup"><span data-stu-id="c807a-188">Remarks</span></span>

* <span data-ttu-id="c807a-189">組織に既定の有効期限ポリシーが適用されている場合を除き、このアクションを使用して作成されたリンクに期限はありません。</span><span class="sxs-lookup"><span data-stu-id="c807a-189">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="c807a-190">リンクはそのアイテムの共有アクセス許可に表示され、アイテムの所有者はそれを削除できます。</span><span class="sxs-lookup"><span data-stu-id="c807a-190">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="c807a-191">リンクは、そのアイテムがチェックアウトされない限り、常にアイテムの現在のバージョンをポイントします (SharePoint の場合のみ)。</span><span class="sxs-lookup"><span data-stu-id="c807a-191">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
} -->
