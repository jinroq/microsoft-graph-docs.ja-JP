---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c21c891981106faa4b631bb2713913bfa8ed0713
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521454"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="98a32-102">SharingLink リソース型</span><span class="sxs-lookup"><span data-stu-id="98a32-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98a32-103">**SharingLink** リソースは、リンク関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="98a32-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="98a32-104">[**Permission**](permission.md) リソースが非 null の **sharingLink** ファセットを持つ場合、アクセス許可は (ユーザーやグループに与えられているアクセス許可ではなく) 共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="98a32-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="98a32-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98a32-105">JSON representation</span></span>

<span data-ttu-id="98a32-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="98a32-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="98a32-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98a32-107">Properties</span></span>

| <span data-ttu-id="98a32-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98a32-108">Property</span></span>       | <span data-ttu-id="98a32-109">型</span><span class="sxs-lookup"><span data-stu-id="98a32-109">Type</span></span>          | <span data-ttu-id="98a32-110">説明</span><span class="sxs-lookup"><span data-stu-id="98a32-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="98a32-111">application</span><span class="sxs-lookup"><span data-stu-id="98a32-111">application</span></span>    | <span data-ttu-id="98a32-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="98a32-112">[identity][]</span></span>  | <span data-ttu-id="98a32-113">リンクが関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="98a32-113">The app the link is associated with.</span></span>
| <span data-ttu-id="98a32-114">type</span><span class="sxs-lookup"><span data-stu-id="98a32-114">type</span></span>           | <span data-ttu-id="98a32-115">String</span><span class="sxs-lookup"><span data-stu-id="98a32-115">String</span></span>        | <span data-ttu-id="98a32-116">作成されたリンクの種類。</span><span class="sxs-lookup"><span data-stu-id="98a32-116">The type of the link created.</span></span>
| <span data-ttu-id="98a32-117">scope</span><span class="sxs-lookup"><span data-stu-id="98a32-117">scope</span></span>          | <span data-ttu-id="98a32-118">String</span><span class="sxs-lookup"><span data-stu-id="98a32-118">String</span></span>        | <span data-ttu-id="98a32-p101">このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="98a32-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="98a32-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="98a32-121">preventsDownload</span></span> | <span data-ttu-id="98a32-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="98a32-122">Boolean</span></span>       | <span data-ttu-id="98a32-123">True の場合、ユーザーは、web 上のアイテムを表示するのにはのみ、このリンクを使用できますし、項目の内容をダウンロードするのには使用できません。</span><span class="sxs-lookup"><span data-stu-id="98a32-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="98a32-124">ビジネスと SharePoint の OneDrive です。</span><span class="sxs-lookup"><span data-stu-id="98a32-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="98a32-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="98a32-125">webHtml</span></span>        | <span data-ttu-id="98a32-126">String</span><span class="sxs-lookup"><span data-stu-id="98a32-126">String</span></span>        | <span data-ttu-id="98a32-127">`embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。</span><span class="sxs-lookup"><span data-stu-id="98a32-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="98a32-128">webUrl</span><span class="sxs-lookup"><span data-stu-id="98a32-128">webUrl</span></span>         | <span data-ttu-id="98a32-129">文字列</span><span class="sxs-lookup"><span data-stu-id="98a32-129">String</span></span>        | <span data-ttu-id="98a32-130">OneDrive の web サイト上で、項目をブラウザーに開く URL です。</span><span class="sxs-lookup"><span data-stu-id="98a32-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="98a32-132">タイプ オプション</span><span class="sxs-lookup"><span data-stu-id="98a32-132">Type options</span></span>

<span data-ttu-id="98a32-133">次の表は、 **type**プロパティの値を定義します。</span><span class="sxs-lookup"><span data-stu-id="98a32-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="98a32-134">値</span><span class="sxs-lookup"><span data-stu-id="98a32-134">Value</span></span>    | <span data-ttu-id="98a32-135">ロール</span><span class="sxs-lookup"><span data-stu-id="98a32-135">Role</span></span>     | <span data-ttu-id="98a32-136">説明</span><span class="sxs-lookup"><span data-stu-id="98a32-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="98a32-137">読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="98a32-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="98a32-138">読み取り/書き込みのアクセスを許可する、編集共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="98a32-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="98a32-139">ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="98a32-139">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="98a32-140">埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。</span><span class="sxs-lookup"><span data-stu-id="98a32-140">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="98a32-141">スコープ オプション</span><span class="sxs-lookup"><span data-stu-id="98a32-141">Scope options</span></span>

<span data-ttu-id="98a32-142">次の表は、**スコープ**のプロパティの値を定義します。</span><span class="sxs-lookup"><span data-stu-id="98a32-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="98a32-143">値</span><span class="sxs-lookup"><span data-stu-id="98a32-143">Value</span></span>            | <span data-ttu-id="98a32-144">説明</span><span class="sxs-lookup"><span data-stu-id="98a32-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="98a32-145">リンクを持つユーザーは、サインインすることがなく、アクセスを持ちます。</span><span class="sxs-lookup"><span data-stu-id="98a32-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="98a32-146">これには、組織の外部ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="98a32-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="98a32-147">アクセス権を取得するのには、組織 (テナント) に署名されたすべてのユーザーのリンクを使用できます。</span><span class="sxs-lookup"><span data-stu-id="98a32-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="98a32-148">ビジネスと SharePoint の OneDrive でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="98a32-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="98a32-149">他の手段を使用して、アイテムへのアクセス権が既に付与されたユーザーだけは、このリンクを使用してアイテムにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="98a32-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="98a32-150">ビジネスと SharePoint の OneDrive でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="98a32-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="98a32-151">リンクでは、特定のユーザーの一覧にのみアクセスが許可されます。</span><span class="sxs-lookup"><span data-stu-id="98a32-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="98a32-152">ビジネスと SharePoint の OneDrive でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="98a32-152">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinglink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
