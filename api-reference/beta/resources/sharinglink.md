---
author: JeremyKelley
description: SharingLink リソースは、リンク関連のデータ項目を単一の構造にグループ化します。
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f1ebff332227410bcb67d87de50a97dd2e078660
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965132"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="5c9f1-103">sharingLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c9f1-103">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c9f1-104">**Sharinglink**リソースは、リンク関連のデータ項目を単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-104">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="5c9f1-105">[**アクセス許可**](permission.md)リソースに非 Null の**sharinglink**ファセットがある場合、アクセス許可は (ユーザーまたはグループに付与されたアクセス許可ではなく) 共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-105">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c9f1-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c9f1-106">JSON representation</span></span>

<span data-ttu-id="5c9f1-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5c9f1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c9f1-108">Properties</span></span>

| <span data-ttu-id="5c9f1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c9f1-109">Property</span></span>       | <span data-ttu-id="5c9f1-110">型</span><span class="sxs-lookup"><span data-stu-id="5c9f1-110">Type</span></span>          | <span data-ttu-id="5c9f1-111">説明</span><span class="sxs-lookup"><span data-stu-id="5c9f1-111">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="5c9f1-112">application</span><span class="sxs-lookup"><span data-stu-id="5c9f1-112">application</span></span>    | <span data-ttu-id="5c9f1-113">[identity][]</span><span class="sxs-lookup"><span data-stu-id="5c9f1-113">[identity][]</span></span>  | <span data-ttu-id="5c9f1-114">リンクが関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-114">The app the link is associated with.</span></span>
| <span data-ttu-id="5c9f1-115">type</span><span class="sxs-lookup"><span data-stu-id="5c9f1-115">type</span></span>           | <span data-ttu-id="5c9f1-116">String</span><span class="sxs-lookup"><span data-stu-id="5c9f1-116">String</span></span>        | <span data-ttu-id="5c9f1-117">作成されたリンクの種類。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-117">The type of the link created.</span></span>
| <span data-ttu-id="5c9f1-118">scope</span><span class="sxs-lookup"><span data-stu-id="5c9f1-118">scope</span></span>          | <span data-ttu-id="5c9f1-119">String</span><span class="sxs-lookup"><span data-stu-id="5c9f1-119">String</span></span>        | <span data-ttu-id="5c9f1-p101">このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="5c9f1-122">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="5c9f1-122">preventsDownload</span></span> | <span data-ttu-id="5c9f1-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c9f1-123">Boolean</span></span>       | <span data-ttu-id="5c9f1-124">True の場合、ユーザーはこのリンクを使用して web 上のアイテムを表示することができ、アイテムのコンテンツをダウンロードするために使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-124">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="5c9f1-125">OneDrive for business と SharePoint の場合のみ。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-125">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="5c9f1-126">webHtml</span><span class="sxs-lookup"><span data-stu-id="5c9f1-126">webHtml</span></span>        | <span data-ttu-id="5c9f1-127">String</span><span class="sxs-lookup"><span data-stu-id="5c9f1-127">String</span></span>        | <span data-ttu-id="5c9f1-128">`embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-128">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="5c9f1-129">webUrl</span><span class="sxs-lookup"><span data-stu-id="5c9f1-129">webUrl</span></span>         | <span data-ttu-id="5c9f1-130">文字列</span><span class="sxs-lookup"><span data-stu-id="5c9f1-130">String</span></span>        | <span data-ttu-id="5c9f1-131">OneDrive の web サイト上で、項目をブラウザーに開く URL です。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-131">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="5c9f1-133">種類のオプション</span><span class="sxs-lookup"><span data-stu-id="5c9f1-133">Type options</span></span>

<span data-ttu-id="5c9f1-134">次の表は、 **type**プロパティに指定できる値を定義します。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-134">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="5c9f1-135">値</span><span class="sxs-lookup"><span data-stu-id="5c9f1-135">Value</span></span>    | <span data-ttu-id="5c9f1-136">ロール</span><span class="sxs-lookup"><span data-stu-id="5c9f1-136">Role</span></span>     | <span data-ttu-id="5c9f1-137">説明</span><span class="sxs-lookup"><span data-stu-id="5c9f1-137">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="5c9f1-138">読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-138">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="5c9f1-139">読み取り/書き込みのアクセスを許可する、編集共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-139">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="5c9f1-p103">ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="5c9f1-142">範囲オプション</span><span class="sxs-lookup"><span data-stu-id="5c9f1-142">Scope options</span></span>

<span data-ttu-id="5c9f1-143">次の表では、 **scope**プロパティに指定できる値を定義します。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-143">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="5c9f1-144">値</span><span class="sxs-lookup"><span data-stu-id="5c9f1-144">Value</span></span>            | <span data-ttu-id="5c9f1-145">説明</span><span class="sxs-lookup"><span data-stu-id="5c9f1-145">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="5c9f1-146">リンクを持つすべてのユーザーが、サインインを必要とせずにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-146">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="5c9f1-147">これには、組織外のユーザーが含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-147">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="5c9f1-148">組織 (テナント) にサインインしているユーザーは、リンクを使用してアクセス権を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-148">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="5c9f1-149">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-149">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="5c9f1-150">他の手段でアイテムへのアクセスが既に許可されているユーザーのみが、このリンクを使用してアイテムにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-150">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="5c9f1-151">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-151">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="5c9f1-152">このリンクは、ユーザーの特定のリストにのみアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-152">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="5c9f1-153">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="5c9f1-153">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
