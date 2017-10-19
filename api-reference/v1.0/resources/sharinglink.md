---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7b7729899d134fa1d5de7debb1f209ec5aadd70d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="e2b9c-102">SharingLink リソース型</span><span class="sxs-lookup"><span data-stu-id="e2b9c-102">SharingLink resource type</span></span>

<span data-ttu-id="e2b9c-103">**SharingLink** リソースは、リンク関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="e2b9c-104">[**Permission**](permission.md) リソースが非 null の **sharingLink** ファセットを持つ場合、アクセス許可は (ユーザーやグループに与えられているアクセス許可ではなく) 共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2b9c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2b9c-105">JSON representation</span></span>

<span data-ttu-id="e2b9c-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e2b9c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2b9c-107">Properties</span></span>

| <span data-ttu-id="e2b9c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2b9c-108">Property</span></span>    | <span data-ttu-id="e2b9c-109">型</span><span class="sxs-lookup"><span data-stu-id="e2b9c-109">Type</span></span>          | <span data-ttu-id="e2b9c-110">説明</span><span class="sxs-lookup"><span data-stu-id="e2b9c-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="e2b9c-111">application</span><span class="sxs-lookup"><span data-stu-id="e2b9c-111">application</span></span> | <span data-ttu-id="e2b9c-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="e2b9c-112">[identity][]</span></span>  | <span data-ttu-id="e2b9c-113">リンクが関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-113">The app the link is associated with.</span></span>
| <span data-ttu-id="e2b9c-114">type</span><span class="sxs-lookup"><span data-stu-id="e2b9c-114">type</span></span>        | <span data-ttu-id="e2b9c-115">String</span><span class="sxs-lookup"><span data-stu-id="e2b9c-115">String</span></span>        | <span data-ttu-id="e2b9c-116">作成されたリンクの種類。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-116">The type of the link created.</span></span>
| <span data-ttu-id="e2b9c-117">scope</span><span class="sxs-lookup"><span data-stu-id="e2b9c-117">scope</span></span>       | <span data-ttu-id="e2b9c-118">String</span><span class="sxs-lookup"><span data-stu-id="e2b9c-118">String</span></span>        | <span data-ttu-id="e2b9c-p101">このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="e2b9c-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="e2b9c-121">webHtml</span></span>     | <span data-ttu-id="e2b9c-122">String</span><span class="sxs-lookup"><span data-stu-id="e2b9c-122">String</span></span>        | <span data-ttu-id="e2b9c-123">`embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-123">For embeddable links, this property contains the HTML code for an  element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="e2b9c-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="e2b9c-124">webUrl</span></span>      | <span data-ttu-id="e2b9c-125">String</span><span class="sxs-lookup"><span data-stu-id="e2b9c-125">String</span></span>        | <span data-ttu-id="e2b9c-126">項目をブラウザーで OneDrive の Web サイト上で開くための URL です。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-enumeration"></a><span data-ttu-id="e2b9c-128">Type 列挙型</span><span class="sxs-lookup"><span data-stu-id="e2b9c-128">Type enumeration</span></span>

<span data-ttu-id="e2b9c-129">この表は、**type** プロパティの可能な値を定義します。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="e2b9c-130">値</span><span class="sxs-lookup"><span data-stu-id="e2b9c-130">Value</span></span>   | <span data-ttu-id="e2b9c-131">ロール</span><span class="sxs-lookup"><span data-stu-id="e2b9c-131">Role</span></span>    | <span data-ttu-id="e2b9c-132">説明</span><span class="sxs-lookup"><span data-stu-id="e2b9c-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="e2b9c-133">読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="e2b9c-134">読み取り/書き込みのアクセスを許可する、編集共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="e2b9c-135">ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-135">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="e2b9c-136">埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-136">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-enumeration"></a><span data-ttu-id="e2b9c-137">スコープ列挙</span><span class="sxs-lookup"><span data-stu-id="e2b9c-137">Scope enumeration</span></span>

| <span data-ttu-id="e2b9c-138">値</span><span class="sxs-lookup"><span data-stu-id="e2b9c-138">Value</span></span>          | <span data-ttu-id="e2b9c-139">説明</span><span class="sxs-lookup"><span data-stu-id="e2b9c-139">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="e2b9c-140">共有リンクは誰でも使用可能です。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-140">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="e2b9c-p103">共有リンクは、同じ組織 (テナント) 内のすべてのユーザーが使用可能です。OneDrive Personal では使用できません。</span><span class="sxs-lookup"><span data-stu-id="e2b9c-p103">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "Facets/SharingLink"
} -->
