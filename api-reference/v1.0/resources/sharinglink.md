---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: SharingLink リソースは、リンク関連のデータ項目を 1 つの構造にグループ化します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 01d27971cd04ff91333d25240e4d1d517e05cec5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034252"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="b2f63-103">SharingLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2f63-103">SharingLink resource type</span></span>

<span data-ttu-id="b2f63-104">**SharingLink** リソースは、リンク関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="b2f63-104">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="b2f63-105">[**Permission**](permission.md) リソースが非 null の **sharingLink** ファセットを持つ場合、アクセス許可は (ユーザーやグループに与えられているアクセス許可ではなく) 共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="b2f63-105">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2f63-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2f63-106">JSON representation</span></span>

<span data-ttu-id="b2f63-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2f63-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="b2f63-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2f63-108">Properties</span></span>

| <span data-ttu-id="b2f63-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2f63-109">Property</span></span>    | <span data-ttu-id="b2f63-110">型</span><span class="sxs-lookup"><span data-stu-id="b2f63-110">Type</span></span>          | <span data-ttu-id="b2f63-111">説明</span><span class="sxs-lookup"><span data-stu-id="b2f63-111">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="b2f63-112">application</span><span class="sxs-lookup"><span data-stu-id="b2f63-112">application</span></span> | <span data-ttu-id="b2f63-113">[identity][]</span><span class="sxs-lookup"><span data-stu-id="b2f63-113">[identity][]</span></span>  | <span data-ttu-id="b2f63-114">リンクが関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="b2f63-114">The app the link is associated with.</span></span>
| <span data-ttu-id="b2f63-115">type</span><span class="sxs-lookup"><span data-stu-id="b2f63-115">type</span></span>        | <span data-ttu-id="b2f63-116">String</span><span class="sxs-lookup"><span data-stu-id="b2f63-116">String</span></span>        | <span data-ttu-id="b2f63-117">作成されたリンクの種類。</span><span class="sxs-lookup"><span data-stu-id="b2f63-117">The type of the link created.</span></span>
| <span data-ttu-id="b2f63-118">scope</span><span class="sxs-lookup"><span data-stu-id="b2f63-118">scope</span></span>       | <span data-ttu-id="b2f63-119">String</span><span class="sxs-lookup"><span data-stu-id="b2f63-119">String</span></span>        | <span data-ttu-id="b2f63-p101">このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="b2f63-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="b2f63-122">webHtml</span><span class="sxs-lookup"><span data-stu-id="b2f63-122">webHtml</span></span>     | <span data-ttu-id="b2f63-123">String</span><span class="sxs-lookup"><span data-stu-id="b2f63-123">String</span></span>        | <span data-ttu-id="b2f63-124">`embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。</span><span class="sxs-lookup"><span data-stu-id="b2f63-124">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="b2f63-125">webUrl</span><span class="sxs-lookup"><span data-stu-id="b2f63-125">webUrl</span></span>      | <span data-ttu-id="b2f63-126">文字列</span><span class="sxs-lookup"><span data-stu-id="b2f63-126">String</span></span>        | <span data-ttu-id="b2f63-127">OneDrive の web サイト上で、項目をブラウザーに開く URL です。</span><span class="sxs-lookup"><span data-stu-id="b2f63-127">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="b2f63-129">種類のオプション</span><span class="sxs-lookup"><span data-stu-id="b2f63-129">Type options</span></span>

<span data-ttu-id="b2f63-130">この表は、**type** プロパティの可能な値を定義します。</span><span class="sxs-lookup"><span data-stu-id="b2f63-130">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="b2f63-131">値</span><span class="sxs-lookup"><span data-stu-id="b2f63-131">Value</span></span>   | <span data-ttu-id="b2f63-132">ロール</span><span class="sxs-lookup"><span data-stu-id="b2f63-132">Role</span></span>    | <span data-ttu-id="b2f63-133">説明</span><span class="sxs-lookup"><span data-stu-id="b2f63-133">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="b2f63-134">読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="b2f63-134">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="b2f63-135">読み取り/書き込みのアクセスを許可する、編集共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="b2f63-135">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="b2f63-p102">ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。</span><span class="sxs-lookup"><span data-stu-id="b2f63-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="b2f63-138">範囲オプション</span><span class="sxs-lookup"><span data-stu-id="b2f63-138">Scope options</span></span>

| <span data-ttu-id="b2f63-139">値</span><span class="sxs-lookup"><span data-stu-id="b2f63-139">Value</span></span>          | <span data-ttu-id="b2f63-140">説明</span><span class="sxs-lookup"><span data-stu-id="b2f63-140">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="b2f63-141">リンクを持つすべてのユーザーが、サインインを必要とせずにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b2f63-141">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="b2f63-142">これには、組織外のユーザーが含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2f63-142">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="b2f63-143">組織 (テナント) にサインインしているユーザーは、リンクを使用してアクセス権を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="b2f63-143">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="b2f63-144">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b2f63-144">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->
