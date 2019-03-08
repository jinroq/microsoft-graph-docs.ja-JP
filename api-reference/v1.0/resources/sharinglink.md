---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: f16f8240800be4b9c1780a4057583381b736f079
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481427"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="cf50a-102">SharingLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf50a-102">SharingLink resource type</span></span>

<span data-ttu-id="cf50a-103">**SharingLink** リソースは、リンク関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="cf50a-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="cf50a-104">[**Permission**](permission.md) リソースが非 null の **sharingLink** ファセットを持つ場合、アクセス許可は (ユーザーやグループに与えられているアクセス許可ではなく) 共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="cf50a-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf50a-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf50a-105">JSON representation</span></span>

<span data-ttu-id="cf50a-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf50a-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cf50a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf50a-107">Properties</span></span>

| <span data-ttu-id="cf50a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf50a-108">Property</span></span>    | <span data-ttu-id="cf50a-109">種類</span><span class="sxs-lookup"><span data-stu-id="cf50a-109">Type</span></span>          | <span data-ttu-id="cf50a-110">説明</span><span class="sxs-lookup"><span data-stu-id="cf50a-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="cf50a-111">application</span><span class="sxs-lookup"><span data-stu-id="cf50a-111">application</span></span> | <span data-ttu-id="cf50a-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="cf50a-112">[identity][]</span></span>  | <span data-ttu-id="cf50a-113">リンクが関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="cf50a-113">The app the link is associated with.</span></span>
| <span data-ttu-id="cf50a-114">type</span><span class="sxs-lookup"><span data-stu-id="cf50a-114">type</span></span>        | <span data-ttu-id="cf50a-115">String</span><span class="sxs-lookup"><span data-stu-id="cf50a-115">String</span></span>        | <span data-ttu-id="cf50a-116">作成されたリンクの種類。</span><span class="sxs-lookup"><span data-stu-id="cf50a-116">The type of the link created.</span></span>
| <span data-ttu-id="cf50a-117">scope</span><span class="sxs-lookup"><span data-stu-id="cf50a-117">scope</span></span>       | <span data-ttu-id="cf50a-118">String
</span><span class="sxs-lookup"><span data-stu-id="cf50a-118">String</span></span>        | <span data-ttu-id="cf50a-p101">このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="cf50a-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="cf50a-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="cf50a-121">webHtml</span></span>     | <span data-ttu-id="cf50a-122">String</span><span class="sxs-lookup"><span data-stu-id="cf50a-122">String</span></span>        | <span data-ttu-id="cf50a-123">`embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。</span><span class="sxs-lookup"><span data-stu-id="cf50a-123">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="cf50a-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="cf50a-124">webUrl</span></span>      | <span data-ttu-id="cf50a-125">文字列</span><span class="sxs-lookup"><span data-stu-id="cf50a-125">String</span></span>        | <span data-ttu-id="cf50a-126">OneDrive の web サイト上で、項目をブラウザーに開く URL です。</span><span class="sxs-lookup"><span data-stu-id="cf50a-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="cf50a-128">種類のオプション</span><span class="sxs-lookup"><span data-stu-id="cf50a-128">Type options</span></span>

<span data-ttu-id="cf50a-129">この表は、**type** プロパティの可能な値を定義します。</span><span class="sxs-lookup"><span data-stu-id="cf50a-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="cf50a-130">値</span><span class="sxs-lookup"><span data-stu-id="cf50a-130">Value</span></span>   | <span data-ttu-id="cf50a-131">ロール</span><span class="sxs-lookup"><span data-stu-id="cf50a-131">Role</span></span>    | <span data-ttu-id="cf50a-132">説明</span><span class="sxs-lookup"><span data-stu-id="cf50a-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="cf50a-133">読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="cf50a-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="cf50a-134">読み取り/書き込みのアクセスを許可する、編集共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="cf50a-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="cf50a-p102">ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。</span><span class="sxs-lookup"><span data-stu-id="cf50a-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="cf50a-137">範囲オプション</span><span class="sxs-lookup"><span data-stu-id="cf50a-137">Scope options</span></span>

| <span data-ttu-id="cf50a-138">値</span><span class="sxs-lookup"><span data-stu-id="cf50a-138">Value</span></span>          | <span data-ttu-id="cf50a-139">説明</span><span class="sxs-lookup"><span data-stu-id="cf50a-139">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="cf50a-140">リンクを持つすべてのユーザーが、サインインを必要とせずにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="cf50a-140">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="cf50a-141">これには、組織外のユーザーが含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf50a-141">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="cf50a-142">組織 (テナント) にサインインしているユーザーは、リンクを使用してアクセス権を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="cf50a-142">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="cf50a-143">OneDrive for business と SharePoint でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="cf50a-143">Only available in OneDrive for Business and SharePoint.</span></span>

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
