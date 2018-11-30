---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルをリンクで共有する
ms.openlocfilehash: 85621a167d3ec3a8ecf9218ceca79367dade76e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071485"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="b2067-102">DriveItem の共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="b2067-102">Create a sharing link for a DriveItem</span></span>

> <span data-ttu-id="b2067-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2067-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2067-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2067-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2067-105">**createLink** アクションを使用して、共有リンクを使って [DriveItem](../resources/driveitem.md) を共有できます。</span><span class="sxs-lookup"><span data-stu-id="b2067-105">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="b2067-p102">**createLink** アクションは、呼び出し元のアプリケーションに指定されたリンクの種類が存在しない場合に、新しい共有リンクを作成します。指定された種類の共有リンクがアプリで既に存在している場合、既存の共有リンクが返されます。</span><span class="sxs-lookup"><span data-stu-id="b2067-p102">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="b2067-108">DriveItem リソースは、そのリソースの先祖から共有アクセス許可を継承します。</span><span class="sxs-lookup"><span data-stu-id="b2067-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2067-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2067-109">Permissions</span></span>

<span data-ttu-id="b2067-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2067-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2067-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2067-112">Permission type</span></span>      | <span data-ttu-id="b2067-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2067-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2067-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2067-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b2067-115">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2067-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2067-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2067-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2067-117">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2067-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2067-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2067-118">Application</span></span> | <span data-ttu-id="b2067-119">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2067-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2067-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2067-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="b2067-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2067-121">Request body</span></span>

<span data-ttu-id="b2067-122">要求本文はアプリケーションが要求する共有リンクのプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="b2067-122">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="b2067-123">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2067-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="b2067-124">名前</span><span class="sxs-lookup"><span data-stu-id="b2067-124">Name</span></span>    |  <span data-ttu-id="b2067-125">型</span><span class="sxs-lookup"><span data-stu-id="b2067-125">Type</span></span>  |                                 <span data-ttu-id="b2067-126">説明</span><span class="sxs-lookup"><span data-stu-id="b2067-126">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="b2067-127">**type**</span><span class="sxs-lookup"><span data-stu-id="b2067-127">**type**</span></span>  | <span data-ttu-id="b2067-128">string</span><span class="sxs-lookup"><span data-stu-id="b2067-128">string</span></span> | <span data-ttu-id="b2067-p105">作成する共有リンクの種類。`view`、`edit`、または `embed` です。</span><span class="sxs-lookup"><span data-stu-id="b2067-p105">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="b2067-131">**scope**</span><span class="sxs-lookup"><span data-stu-id="b2067-131">**scope**</span></span> | <span data-ttu-id="b2067-132">string</span><span class="sxs-lookup"><span data-stu-id="b2067-132">string</span></span> | <span data-ttu-id="b2067-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b2067-133">Optional.</span></span> <span data-ttu-id="b2067-134">作成するリンクのスコープ。</span><span class="sxs-lookup"><span data-stu-id="b2067-134">The scope of link to create.</span></span> <span data-ttu-id="b2067-135">`anonymous` または `organization` のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="b2067-135">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="b2067-136">リンクの種類</span><span class="sxs-lookup"><span data-stu-id="b2067-136">Link types</span></span>

<span data-ttu-id="b2067-137">**type** パラメーターには次の値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b2067-137">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="b2067-138">種類の値</span><span class="sxs-lookup"><span data-stu-id="b2067-138">Type value</span></span> | <span data-ttu-id="b2067-139">説明</span><span class="sxs-lookup"><span data-stu-id="b2067-139">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="b2067-140">その DriveItem への読み取り専用リンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2067-140">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="b2067-141">その DriveItem への読み取り/書き込みリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2067-141">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="b2067-142">その DriveItem への埋め込み可能なリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2067-142">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="b2067-143">このオプションは OneDrive 個人用のファイルでのみ選択可能です。</span><span class="sxs-lookup"><span data-stu-id="b2067-143">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="b2067-144">スコープの種類</span><span class="sxs-lookup"><span data-stu-id="b2067-144">Scope types</span></span>

<span data-ttu-id="b2067-145">**scope** パラメーターには次の値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b2067-145">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="b2067-146">**scope** パラメーターが指定されていない場合、組織の既定のリンクの種類が作成されます。</span><span class="sxs-lookup"><span data-stu-id="b2067-146">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="b2067-147">種類の値</span><span class="sxs-lookup"><span data-stu-id="b2067-147">Type value</span></span>     | <span data-ttu-id="b2067-148">説明</span><span class="sxs-lookup"><span data-stu-id="b2067-148">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="b2067-149">DriveItem への、すべてのユーザーがアクセス可能なリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2067-149">Creates a link to the DriveItem accessible to anyone with the link.</span></span> <span data-ttu-id="b2067-150">匿名リンクは管理者により無効にされることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2067-150">Anonymous links may be disabled by an administrator.</span></span>                 |
| `organization` | <span data-ttu-id="b2067-151">DriveItem への、ユーザーの組織内のだれでもアクセス可能なリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2067-151">Creates a link to the DriveItem accessible to anyone within the user's organization.</span></span> <span data-ttu-id="b2067-152">組織のリンク スコープは、OneDrive 個人用では使用できません。</span><span class="sxs-lookup"><span data-stu-id="b2067-152">Organization link scope is not available for OneDrive personal.</span></span> |

## <a name="response"></a><span data-ttu-id="b2067-153">応答</span><span class="sxs-lookup"><span data-stu-id="b2067-153">Response</span></span>

<span data-ttu-id="b2067-154">正常に実行されると、このメソッドは要求された共有アクセス許可を表す応答本文で、単一の[アクセス許可](../resources/permission.md)リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="b2067-154">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="b2067-155">応答は、アイテムに新しい共有リンクが作成される場合は `201 Created`、既存のリンクが返される場合は `200 OK` となります。</span><span class="sxs-lookup"><span data-stu-id="b2067-155">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="b2067-156">例</span><span class="sxs-lookup"><span data-stu-id="b2067-156">Example</span></span>

<span data-ttu-id="b2067-157">次の例では、ユーザーの OneDrive の {itemId} で指定された DriveItem に対して共有リンクを作成することを要求します。</span><span class="sxs-lookup"><span data-stu-id="b2067-157">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="b2067-158">共有リンクは、読み取り専用でそのリンクによってだれでも使用可能になるよう構成されます。</span><span class="sxs-lookup"><span data-stu-id="b2067-158">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="b2067-159">要求</span><span class="sxs-lookup"><span data-stu-id="b2067-159">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a><span data-ttu-id="b2067-160">応答</span><span class="sxs-lookup"><span data-stu-id="b2067-160">Response</span></span>

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

## <a name="creating-company-sharable-links"></a><span data-ttu-id="b2067-161">会社の共有可能リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="b2067-161">Creating company sharable links</span></span>

<span data-ttu-id="b2067-162">OneDrive for Business および SharePoint は、会社の共有可能リンクをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="b2067-162">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="b2067-163">これらは匿名リンクに似ていますが、所有組織のメンバーだけが使用できる点が異なります。</span><span class="sxs-lookup"><span data-stu-id="b2067-163">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="b2067-164">会社の共有可能リンクを作成するには、**scope** パラメーターで値 `organization` を指定して使用します。</span><span class="sxs-lookup"><span data-stu-id="b2067-164">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="b2067-165">要求</span><span class="sxs-lookup"><span data-stu-id="b2067-165">Request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a><span data-ttu-id="b2067-166">応答</span><span class="sxs-lookup"><span data-stu-id="b2067-166">Response</span></span>

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

## <a name="creating-embeddable-links"></a><span data-ttu-id="b2067-167">埋め込み可能なリンクを作成する</span><span class="sxs-lookup"><span data-stu-id="b2067-167">Creating embeddable links</span></span>

<span data-ttu-id="b2067-p113">リンクの種類で `embed` を使用する場合、返される webUrl は `<iframe>` HTML 要素に埋め込むことができます。埋め込みリンクが作成されると、`webHtml` プロパティに `<iframe>` がコンテンツをホストするための HTML コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b2067-p113">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="b2067-170">**注:** 埋め込みリンクは、OneDrive 個人用でのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="b2067-170">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="b2067-171">要求</span><span class="sxs-lookup"><span data-stu-id="b2067-171">Request</span></span>

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a><span data-ttu-id="b2067-172">応答</span><span class="sxs-lookup"><span data-stu-id="b2067-172">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="b2067-173">注釈</span><span class="sxs-lookup"><span data-stu-id="b2067-173">Remarks</span></span>

* <span data-ttu-id="b2067-174">組織に既定の有効期限ポリシーが適用されている場合を除き、このアクションを使用して作成されたリンクに期限はありません。</span><span class="sxs-lookup"><span data-stu-id="b2067-174">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="b2067-175">リンクはそのアイテムの共有アクセス許可に表示され、アイテムの所有者はそれを削除できます。</span><span class="sxs-lookup"><span data-stu-id="b2067-175">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="b2067-176">リンクは、そのアイテムがチェックアウトされない限り、常にアイテムの現在のバージョンをポイントします (SharePoint の場合のみ)。</span><span class="sxs-lookup"><span data-stu-id="b2067-176">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link"
} -->