---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルをリンクで共有する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 249b67852d4b796be465c79cadde9b07d97f695a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713179"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="4d0e0-102">DriveItem の共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="4d0e0-102">Create a sharing link for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d0e0-103">**createLink** アクションを使用して、共有リンクを使って [DriveItem](../resources/driveitem.md) を共有できます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-103">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="4d0e0-p101">**createLink** アクションは、呼び出し元のアプリケーションに指定されたリンクの種類が存在しない場合に、新しい共有リンクを作成します。指定された種類の共有リンクがアプリで既に存在している場合、既存の共有リンクが返されます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="4d0e0-106">DriveItem リソースは、そのリソースの先祖から共有アクセス許可を継承します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-106">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d0e0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d0e0-107">Permissions</span></span>

<span data-ttu-id="4d0e0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d0e0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d0e0-110">Permission type</span></span>      | <span data-ttu-id="4d0e0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d0e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d0e0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d0e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4d0e0-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d0e0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d0e0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d0e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d0e0-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d0e0-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d0e0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d0e0-116">Application</span></span> | <span data-ttu-id="4d0e0-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d0e0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d0e0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d0e0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="4d0e0-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d0e0-119">Request body</span></span>

<span data-ttu-id="4d0e0-120">要求本文はアプリケーションが要求する共有リンクのプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-120">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="4d0e0-121">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-121">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="4d0e0-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d0e0-122">Property</span></span>                 |  <span data-ttu-id="4d0e0-123">型</span><span class="sxs-lookup"><span data-stu-id="4d0e0-123">Type</span></span>  |                                 <span data-ttu-id="4d0e0-124">説明</span><span class="sxs-lookup"><span data-stu-id="4d0e0-124">Description</span></span>                                                               |
| :----------------------| :----- | :---------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4d0e0-125">type</span><span class="sxs-lookup"><span data-stu-id="4d0e0-125">type</span></span>               | <span data-ttu-id="4d0e0-126">string</span><span class="sxs-lookup"><span data-stu-id="4d0e0-126">string</span></span> | <span data-ttu-id="4d0e0-127">作成する共有リンクの種類。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-127">The type of sharing link to create.</span></span> <span data-ttu-id="4d0e0-128">表示、編集、または埋め込みのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-128">Either view, edit, or embed.</span></span>                                    |
|<span data-ttu-id="4d0e0-129">password</span><span class="sxs-lookup"><span data-stu-id="4d0e0-129">password</span></span>           | <span data-ttu-id="4d0e0-130">string</span><span class="sxs-lookup"><span data-stu-id="4d0e0-130">string</span></span> | <span data-ttu-id="4d0e0-131">作成者によって設定された共有リンクのパスワード。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-131">The password of the sharing link that is set by the creator.</span></span> <span data-ttu-id="4d0e0-132">省略可能および OneDrive 個人用のみ。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-132">Optional and OneDrive Personal only.</span></span>         |
|<span data-ttu-id="4d0e0-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4d0e0-133">expirationDateTime</span></span> | <span data-ttu-id="4d0e0-134">string</span><span class="sxs-lookup"><span data-stu-id="4d0e0-134">string</span></span> | <span data-ttu-id="4d0e0-135">Yyyy-mm-ddthh: mm: ssZ DateTime の形式の文字列は、アクセス許可の有効期限を示します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-135">A String with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span> |
|<span data-ttu-id="4d0e0-136">scope</span><span class="sxs-lookup"><span data-stu-id="4d0e0-136">scope</span></span>              | <span data-ttu-id="4d0e0-137">string</span><span class="sxs-lookup"><span data-stu-id="4d0e0-137">string</span></span> | <span data-ttu-id="4d0e0-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-138">Optional.</span></span> <span data-ttu-id="4d0e0-139">作成するリンクのスコープ。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-139">The scope of link to create.</span></span> <span data-ttu-id="4d0e0-140">匿名または組織のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-140">Either anonymous or organization.</span></span>                              |


### <a name="link-types"></a><span data-ttu-id="4d0e0-141">リンクの種類</span><span class="sxs-lookup"><span data-stu-id="4d0e0-141">Link types</span></span>

<span data-ttu-id="4d0e0-142">**type** パラメーターには次の値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-142">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="4d0e0-143">種類の値</span><span class="sxs-lookup"><span data-stu-id="4d0e0-143">Type value</span></span> | <span data-ttu-id="4d0e0-144">説明</span><span class="sxs-lookup"><span data-stu-id="4d0e0-144">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| <span data-ttu-id="4d0e0-145">ビュー</span><span class="sxs-lookup"><span data-stu-id="4d0e0-145">view</span></span>     | <span data-ttu-id="4d0e0-146">その DriveItem への読み取り専用リンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-146">Creates a read-only link to the DriveItem.</span></span>                                                        |
| <span data-ttu-id="4d0e0-147">edit</span><span class="sxs-lookup"><span data-stu-id="4d0e0-147">edit</span></span>     | <span data-ttu-id="4d0e0-148">その DriveItem への読み取り/書き込みリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-148">Creates a read-write link to the DriveItem.</span></span>                                                       |
| <span data-ttu-id="4d0e0-149">埋め込み</span><span class="sxs-lookup"><span data-stu-id="4d0e0-149">embed</span></span>    | <span data-ttu-id="4d0e0-150">その DriveItem への埋め込み可能なリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-150">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="4d0e0-151">このオプションは OneDrive 個人用のファイルでのみ選択可能です。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-151">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="4d0e0-152">スコープの種類</span><span class="sxs-lookup"><span data-stu-id="4d0e0-152">Scope types</span></span>

<span data-ttu-id="4d0e0-153">**scope** パラメーターには次の値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-153">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="4d0e0-154">**scope** パラメーターが指定されていない場合、組織の既定のリンクの種類が作成されます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-154">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="4d0e0-155">値</span><span class="sxs-lookup"><span data-stu-id="4d0e0-155">Value</span></span>          | <span data-ttu-id="4d0e0-156">説明</span><span class="sxs-lookup"><span data-stu-id="4d0e0-156">Description</span></span>
|:---------------|:------------------------------------------------------------
| <span data-ttu-id="4d0e0-157">匿名</span><span class="sxs-lookup"><span data-stu-id="4d0e0-157">anonymous</span></span>    | <span data-ttu-id="4d0e0-158">リンクを持つすべてのユーザーが、サインインを必要とせずにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-158">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="4d0e0-159">これには、組織外のユーザーが含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-159">This may include people outside of your organization.</span></span> <span data-ttu-id="4d0e0-160">匿名リンクのサポートは、管理者によって無効にされている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-160">Anonymous link support may be disabled by an administrator.</span></span>
| <span data-ttu-id="4d0e0-161">組織</span><span class="sxs-lookup"><span data-stu-id="4d0e0-161">organization</span></span> | <span data-ttu-id="4d0e0-162">組織 (テナント) にサインインしているユーザーは、リンクを使用してアクセス権を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-162">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="4d0e0-163">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-163">Only available in OneDrive for Business and SharePoint.</span></span>


## <a name="response"></a><span data-ttu-id="4d0e0-164">応答</span><span class="sxs-lookup"><span data-stu-id="4d0e0-164">Response</span></span>

<span data-ttu-id="4d0e0-165">正常に実行されると、このメソッドは要求された共有アクセス許可を表す応答本文で、単一の[アクセス許可](../resources/permission.md)リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-165">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="4d0e0-166">応答は、アイテムに新しい共有リンクが作成される場合は `201 Created`、既存のリンクが返される場合は `200 OK` となります。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-166">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="4d0e0-167">例</span><span class="sxs-lookup"><span data-stu-id="4d0e0-167">Example</span></span>

<span data-ttu-id="4d0e0-168">次の例では、ユーザーの OneDrive の {itemId} で指定された DriveItem に対して共有リンクを作成することを要求します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-168">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="4d0e0-169">共有リンクは、読み取り専用でそのリンクによってだれでも使用可能になるよう構成されます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-169">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="4d0e0-170">要求</span><span class="sxs-lookup"><span data-stu-id="4d0e0-170">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4d0e0-171">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4d0e0-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "password": "ThisIsMyPrivatePassword",
  "scope": "anonymous"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d0e0-172">C#</span><span class="sxs-lookup"><span data-stu-id="4d0e0-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d0e0-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d0e0-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d0e0-174">目的-C</span><span class="sxs-lookup"><span data-stu-id="4d0e0-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d0e0-175">応答</span><span class="sxs-lookup"><span data-stu-id="4d0e0-175">Response</span></span>

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
  },
  "hasPassword": true
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="4d0e0-176">会社の共有可能リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="4d0e0-176">Creating company sharable links</span></span>

<span data-ttu-id="4d0e0-177">OneDrive for Business および SharePoint は、会社の共有可能リンクをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-177">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="4d0e0-178">これらは匿名リンクに似ていますが、所有組織のメンバーだけが使用できる点が異なります。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-178">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="4d0e0-179">会社の共有可能リンクを作成するには、**scope** パラメーターで値 `organization` を指定して使用します。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-179">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="4d0e0-180">要求</span><span class="sxs-lookup"><span data-stu-id="4d0e0-180">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4d0e0-181">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4d0e0-181">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d0e0-182">C#</span><span class="sxs-lookup"><span data-stu-id="4d0e0-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d0e0-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d0e0-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d0e0-184">目的-C</span><span class="sxs-lookup"><span data-stu-id="4d0e0-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d0e0-185">応答</span><span class="sxs-lookup"><span data-stu-id="4d0e0-185">Response</span></span>

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

## <a name="creating-embeddable-links"></a><span data-ttu-id="4d0e0-186">埋め込み可能なリンクを作成する</span><span class="sxs-lookup"><span data-stu-id="4d0e0-186">Creating embeddable links</span></span>

<span data-ttu-id="4d0e0-p113">リンクの種類で `embed` を使用する場合、返される webUrl は `<iframe>` HTML 要素に埋め込むことができます。埋め込みリンクが作成されると、`webHtml` プロパティに `<iframe>` がコンテンツをホストするための HTML コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-p113">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="4d0e0-189">**注:** 埋め込みリンクは、OneDrive 個人用でのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-189">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="4d0e0-190">要求</span><span class="sxs-lookup"><span data-stu-id="4d0e0-190">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4d0e0-191">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4d0e0-191">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d0e0-192">C#</span><span class="sxs-lookup"><span data-stu-id="4d0e0-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d0e0-193">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d0e0-193">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d0e0-194">目的-C</span><span class="sxs-lookup"><span data-stu-id="4d0e0-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d0e0-195">応答</span><span class="sxs-lookup"><span data-stu-id="4d0e0-195">Response</span></span>

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
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="4d0e0-196">注釈</span><span class="sxs-lookup"><span data-stu-id="4d0e0-196">Remarks</span></span>

* <span data-ttu-id="4d0e0-197">組織に既定の有効期限ポリシーが適用されている場合を除き、このアクションを使用して作成されたリンクに期限はありません。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-197">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="4d0e0-198">リンクはそのアイテムの共有アクセス許可に表示され、アイテムの所有者はそれを削除できます。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-198">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="4d0e0-199">リンクは、そのアイテムがチェックアウトされない限り、常にアイテムの現在のバージョンをポイントします (SharePoint の場合のみ)。</span><span class="sxs-lookup"><span data-stu-id="4d0e0-199">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->
