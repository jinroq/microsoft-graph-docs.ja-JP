---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
description: SharePointIds リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。
doc_type: resourcePageType
ms.openlocfilehash: a7dfd936770ac85b458cb8b086ff05e328d2ea9c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034280"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="430fe-103">SharePointIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="430fe-103">SharePointIds resource type</span></span>

<span data-ttu-id="430fe-104">**SharePointIds** リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="430fe-104">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="430fe-105">**注:** 個人用の OneDrive から返されたアイテムには **SharePointIds** ファセットは含まれません。</span><span class="sxs-lookup"><span data-stu-id="430fe-105">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="430fe-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="430fe-106">JSON representation</span></span>

<span data-ttu-id="430fe-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="430fe-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="430fe-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="430fe-108">Properties</span></span>

| <span data-ttu-id="430fe-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="430fe-109">Property</span></span>         | <span data-ttu-id="430fe-110">型</span><span class="sxs-lookup"><span data-stu-id="430fe-110">Type</span></span>         | <span data-ttu-id="430fe-111">説明</span><span class="sxs-lookup"><span data-stu-id="430fe-111">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="430fe-112">listId</span><span class="sxs-lookup"><span data-stu-id="430fe-112">listId</span></span>           | <span data-ttu-id="430fe-113">string</span><span class="sxs-lookup"><span data-stu-id="430fe-113">string</span></span>       | <span data-ttu-id="430fe-114">SharePoint 内にあるアイテムの一覧の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="430fe-114">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="430fe-115">listItemId</span><span class="sxs-lookup"><span data-stu-id="430fe-115">listItemId</span></span>       | <span data-ttu-id="430fe-116">string</span><span class="sxs-lookup"><span data-stu-id="430fe-116">string</span></span>       | <span data-ttu-id="430fe-117">含まれているリスト内にあるアイテムの整数の識別子。</span><span class="sxs-lookup"><span data-stu-id="430fe-117">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="430fe-118">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="430fe-118">listItemUniqueId</span></span> | <span data-ttu-id="430fe-119">string</span><span class="sxs-lookup"><span data-stu-id="430fe-119">string</span></span>       | <span data-ttu-id="430fe-120">OneDrive for Business または SharePoint サイト内のアイテムの一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="430fe-120">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="430fe-121">siteId</span><span class="sxs-lookup"><span data-stu-id="430fe-121">siteId</span></span>           | <span data-ttu-id="430fe-122">string</span><span class="sxs-lookup"><span data-stu-id="430fe-122">string</span></span>       | <span data-ttu-id="430fe-123">アイテムのサイト コレクション (SPSite) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="430fe-123">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="430fe-124">siteUrl</span><span class="sxs-lookup"><span data-stu-id="430fe-124">siteUrl</span></span>          | <span data-ttu-id="430fe-125">string (URL)</span><span class="sxs-lookup"><span data-stu-id="430fe-125">string (url)</span></span> | <span data-ttu-id="430fe-126">アイテムが含まれるサイトの SharePoint URL です。</span><span class="sxs-lookup"><span data-stu-id="430fe-126">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="430fe-127">webId</span><span class="sxs-lookup"><span data-stu-id="430fe-127">webId</span></span>            | <span data-ttu-id="430fe-128">string</span><span class="sxs-lookup"><span data-stu-id="430fe-128">string</span></span>       | <span data-ttu-id="430fe-129">アイテムのサイト (SPWeb) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="430fe-129">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="430fe-130">備考</span><span class="sxs-lookup"><span data-stu-id="430fe-130">Remarks</span></span>

<span data-ttu-id="430fe-131">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="430fe-131">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
