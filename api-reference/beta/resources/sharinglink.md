---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c303436aafbdbb5167a992f405036b5e00e4d635
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856393"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="6129e-102">sharingLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6129e-102">sharingLink resource type</span></span>

> <span data-ttu-id="6129e-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6129e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6129e-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6129e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6129e-105">**SharingLink**リソースでは、1 つの構造体にデータのリンクに関連する項目をグループ化します。</span><span class="sxs-lookup"><span data-stu-id="6129e-105">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="6129e-106">[**アクセス許可**](permission.md)リソースに非 null **sharingLink**ファセットがある場合、アクセス許可 (アクセス許可がユーザーまたはグループに与えられている) ではなく共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="6129e-106">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6129e-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6129e-107">JSON representation</span></span>

<span data-ttu-id="6129e-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6129e-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6129e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6129e-109">Properties</span></span>

| <span data-ttu-id="6129e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6129e-110">Property</span></span>       | <span data-ttu-id="6129e-111">種類</span><span class="sxs-lookup"><span data-stu-id="6129e-111">Type</span></span>          | <span data-ttu-id="6129e-112">説明</span><span class="sxs-lookup"><span data-stu-id="6129e-112">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="6129e-113">application</span><span class="sxs-lookup"><span data-stu-id="6129e-113">application</span></span>    | <span data-ttu-id="6129e-114">[identity][]</span><span class="sxs-lookup"><span data-stu-id="6129e-114">[identity][]</span></span>  | <span data-ttu-id="6129e-115">リンクが関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="6129e-115">The app the link is associated with.</span></span>
| <span data-ttu-id="6129e-116">type</span><span class="sxs-lookup"><span data-stu-id="6129e-116">type</span></span>           | <span data-ttu-id="6129e-117">String</span><span class="sxs-lookup"><span data-stu-id="6129e-117">String</span></span>        | <span data-ttu-id="6129e-118">作成されたリンクの種類。</span><span class="sxs-lookup"><span data-stu-id="6129e-118">The type of the link created.</span></span>
| <span data-ttu-id="6129e-119">scope</span><span class="sxs-lookup"><span data-stu-id="6129e-119">scope</span></span>          | <span data-ttu-id="6129e-120">String</span><span class="sxs-lookup"><span data-stu-id="6129e-120">String</span></span>        | <span data-ttu-id="6129e-p102">このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="6129e-p102">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="6129e-123">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="6129e-123">preventsDownload</span></span> | <span data-ttu-id="6129e-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="6129e-124">Boolean</span></span>       | <span data-ttu-id="6129e-125">True の場合、ユーザーは、web 上のアイテムを表示するのにはのみ、このリンクを使用できますし、項目の内容をダウンロードするのには使用できません。</span><span class="sxs-lookup"><span data-stu-id="6129e-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="6129e-126">ビジネスと SharePoint の OneDrive です。</span><span class="sxs-lookup"><span data-stu-id="6129e-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="6129e-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="6129e-127">webHtml</span></span>        | <span data-ttu-id="6129e-128">String</span><span class="sxs-lookup"><span data-stu-id="6129e-128">String</span></span>        | <span data-ttu-id="6129e-129">`embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。</span><span class="sxs-lookup"><span data-stu-id="6129e-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="6129e-130">webUrl</span><span class="sxs-lookup"><span data-stu-id="6129e-130">webUrl</span></span>         | <span data-ttu-id="6129e-131">String</span><span class="sxs-lookup"><span data-stu-id="6129e-131">String</span></span>        | <span data-ttu-id="6129e-132">OneDrive の web サイト上で、項目をブラウザーに開く URL です。</span><span class="sxs-lookup"><span data-stu-id="6129e-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="6129e-134">タイプ オプション</span><span class="sxs-lookup"><span data-stu-id="6129e-134">Type options</span></span>

<span data-ttu-id="6129e-135">次の表は、 **type**プロパティの値を定義します。</span><span class="sxs-lookup"><span data-stu-id="6129e-135">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="6129e-136">値</span><span class="sxs-lookup"><span data-stu-id="6129e-136">Value</span></span>    | <span data-ttu-id="6129e-137">ロール</span><span class="sxs-lookup"><span data-stu-id="6129e-137">Role</span></span>     | <span data-ttu-id="6129e-138">説明</span><span class="sxs-lookup"><span data-stu-id="6129e-138">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="6129e-139">読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="6129e-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="6129e-140">読み取り/書き込みのアクセスを許可する、編集共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="6129e-140">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="6129e-141">ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="6129e-141">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="6129e-142">埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。</span><span class="sxs-lookup"><span data-stu-id="6129e-142">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="6129e-143">スコープ オプション</span><span class="sxs-lookup"><span data-stu-id="6129e-143">Scope options</span></span>

<span data-ttu-id="6129e-144">次の表は、**スコープ**のプロパティの値を定義します。</span><span class="sxs-lookup"><span data-stu-id="6129e-144">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="6129e-145">値</span><span class="sxs-lookup"><span data-stu-id="6129e-145">Value</span></span>            | <span data-ttu-id="6129e-146">説明</span><span class="sxs-lookup"><span data-stu-id="6129e-146">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="6129e-147">リンクを持つユーザーは、サインインすることがなく、アクセスを持ちます。</span><span class="sxs-lookup"><span data-stu-id="6129e-147">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="6129e-148">これには、組織の外部ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6129e-148">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="6129e-149">アクセス権を取得するのには、組織 (テナント) に署名されたすべてのユーザーのリンクを使用できます。</span><span class="sxs-lookup"><span data-stu-id="6129e-149">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="6129e-150">ビジネスと SharePoint の OneDrive でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="6129e-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="6129e-151">他の手段を使用して、アイテムへのアクセス権が既に付与されたユーザーだけは、このリンクを使用してアイテムにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="6129e-151">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="6129e-152">ビジネスと SharePoint の OneDrive でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="6129e-152">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="6129e-153">リンクでは、特定のユーザーの一覧にのみアクセスが許可されます。</span><span class="sxs-lookup"><span data-stu-id="6129e-153">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="6129e-154">ビジネスと SharePoint の OneDrive でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="6129e-154">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": ""
}-->
