---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: 7f0ecdbb498ee75133ec9499027f7cfdc6191327
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583824"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="ae8f7-102">sharinglink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae8f7-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae8f7-103">**sharinglink**リソースは、リンク関連のデータ項目を単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="ae8f7-104">[**アクセス許可**](permission.md)リソースに非 null の**sharinglink**ファセットがある場合、アクセス許可は (ユーザーまたはグループに付与されたアクセス許可ではなく) 共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae8f7-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae8f7-105">JSON representation</span></span>

<span data-ttu-id="ae8f7-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ae8f7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae8f7-107">Properties</span></span>

| <span data-ttu-id="ae8f7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae8f7-108">Property</span></span>       | <span data-ttu-id="ae8f7-109">型</span><span class="sxs-lookup"><span data-stu-id="ae8f7-109">Type</span></span>          | <span data-ttu-id="ae8f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="ae8f7-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="ae8f7-111">application</span><span class="sxs-lookup"><span data-stu-id="ae8f7-111">application</span></span>    | <span data-ttu-id="ae8f7-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="ae8f7-112">[identity][]</span></span>  | <span data-ttu-id="ae8f7-113">リンクが関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-113">The app the link is associated with.</span></span>
| <span data-ttu-id="ae8f7-114">type</span><span class="sxs-lookup"><span data-stu-id="ae8f7-114">type</span></span>           | <span data-ttu-id="ae8f7-115">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-115">String</span></span>        | <span data-ttu-id="ae8f7-116">作成されたリンクの種類。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-116">The type of the link created.</span></span>
| <span data-ttu-id="ae8f7-117">scope</span><span class="sxs-lookup"><span data-stu-id="ae8f7-117">scope</span></span>          | <span data-ttu-id="ae8f7-118">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-118">String</span></span>        | <span data-ttu-id="ae8f7-p101">このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="ae8f7-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="ae8f7-121">preventsDownload</span></span> | <span data-ttu-id="ae8f7-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae8f7-122">Boolean</span></span>       | <span data-ttu-id="ae8f7-123">true の場合、ユーザーはこのリンクを使用して web 上のアイテムを表示することができ、アイテムのコンテンツをダウンロードするために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="ae8f7-124">OneDrive for business と SharePoint の場合のみ。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="ae8f7-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="ae8f7-125">webHtml</span></span>        | <span data-ttu-id="ae8f7-126">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-126">String</span></span>        | <span data-ttu-id="ae8f7-127">`embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="ae8f7-128">webUrl</span><span class="sxs-lookup"><span data-stu-id="ae8f7-128">webUrl</span></span>         | <span data-ttu-id="ae8f7-129">文字列</span><span class="sxs-lookup"><span data-stu-id="ae8f7-129">String</span></span>        | <span data-ttu-id="ae8f7-130">OneDrive の web サイト上で、項目をブラウザーに開く URL です。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="ae8f7-132">種類のオプション</span><span class="sxs-lookup"><span data-stu-id="ae8f7-132">Type options</span></span>

<span data-ttu-id="ae8f7-133">次の表は、 **type**プロパティに指定できる値を定義します。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="ae8f7-134">値</span><span class="sxs-lookup"><span data-stu-id="ae8f7-134">Value</span></span>    | <span data-ttu-id="ae8f7-135">ロール</span><span class="sxs-lookup"><span data-stu-id="ae8f7-135">Role</span></span>     | <span data-ttu-id="ae8f7-136">説明</span><span class="sxs-lookup"><span data-stu-id="ae8f7-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="ae8f7-137">読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="ae8f7-138">読み取り/書き込みのアクセスを許可する、編集共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="ae8f7-p103">ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="ae8f7-141">範囲オプション</span><span class="sxs-lookup"><span data-stu-id="ae8f7-141">Scope options</span></span>

<span data-ttu-id="ae8f7-142">次の表では、 **scope**プロパティに指定できる値を定義します。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="ae8f7-143">値</span><span class="sxs-lookup"><span data-stu-id="ae8f7-143">Value</span></span>            | <span data-ttu-id="ae8f7-144">説明</span><span class="sxs-lookup"><span data-stu-id="ae8f7-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="ae8f7-145">リンクを持つすべてのユーザーが、サインインを必要とせずにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="ae8f7-146">これには、組織外のユーザーが含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="ae8f7-147">組織 (テナント) にサインインしているユーザーは、リンクを使用してアクセス権を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="ae8f7-148">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="ae8f7-149">他の手段でアイテムへのアクセスが既に許可されているユーザーのみが、このリンクを使用してアイテムにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="ae8f7-150">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="ae8f7-151">このリンクは、ユーザーの特定のリストにのみアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="ae8f7-152">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ae8f7-152">Only available in OneDrive for Business and SharePoint.</span></span>

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
