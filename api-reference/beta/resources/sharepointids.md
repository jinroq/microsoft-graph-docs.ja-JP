---
author: JeremyKelley
description: SharePointIds リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c7e18e43bcbe9c73500701577c752e7a30d47194
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965125"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="ded1b-103">SharePointIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ded1b-103">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ded1b-104">**SharePointIds** リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="ded1b-104">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="ded1b-105">**注:** 個人用の OneDrive から返されたアイテムには **SharePointIds** ファセットは含まれません。</span><span class="sxs-lookup"><span data-stu-id="ded1b-105">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ded1b-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ded1b-106">JSON representation</span></span>

<span data-ttu-id="ded1b-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ded1b-107">Here is a JSON representation of the resource</span></span>

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
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="ded1b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ded1b-108">Properties</span></span>

| <span data-ttu-id="ded1b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ded1b-109">Property</span></span>         | <span data-ttu-id="ded1b-110">型</span><span class="sxs-lookup"><span data-stu-id="ded1b-110">Type</span></span>         | <span data-ttu-id="ded1b-111">説明</span><span class="sxs-lookup"><span data-stu-id="ded1b-111">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="ded1b-112">listId</span><span class="sxs-lookup"><span data-stu-id="ded1b-112">listId</span></span>           | <span data-ttu-id="ded1b-113">string</span><span class="sxs-lookup"><span data-stu-id="ded1b-113">string</span></span>       | <span data-ttu-id="ded1b-114">SharePoint 内にあるアイテムの一覧の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="ded1b-114">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="ded1b-115">listItemId</span><span class="sxs-lookup"><span data-stu-id="ded1b-115">listItemId</span></span>       | <span data-ttu-id="ded1b-116">string</span><span class="sxs-lookup"><span data-stu-id="ded1b-116">string</span></span>       | <span data-ttu-id="ded1b-117">含まれているリスト内にあるアイテムの整数の識別子。</span><span class="sxs-lookup"><span data-stu-id="ded1b-117">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="ded1b-118">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="ded1b-118">listItemUniqueId</span></span> | <span data-ttu-id="ded1b-119">string</span><span class="sxs-lookup"><span data-stu-id="ded1b-119">string</span></span>       | <span data-ttu-id="ded1b-120">OneDrive for Business または SharePoint サイト内のアイテムの一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="ded1b-120">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="ded1b-121">siteId</span><span class="sxs-lookup"><span data-stu-id="ded1b-121">siteId</span></span>           | <span data-ttu-id="ded1b-122">string</span><span class="sxs-lookup"><span data-stu-id="ded1b-122">string</span></span>       | <span data-ttu-id="ded1b-123">アイテムのサイト コレクション (SPSite) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="ded1b-123">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="ded1b-124">siteUrl</span><span class="sxs-lookup"><span data-stu-id="ded1b-124">siteUrl</span></span>          | <span data-ttu-id="ded1b-125">string (URL)</span><span class="sxs-lookup"><span data-stu-id="ded1b-125">string (url)</span></span> | <span data-ttu-id="ded1b-126">アイテムが含まれるサイトの SharePoint URL です。</span><span class="sxs-lookup"><span data-stu-id="ded1b-126">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="ded1b-127">tenantId</span><span class="sxs-lookup"><span data-stu-id="ded1b-127">tenantId</span></span>         | <span data-ttu-id="ded1b-128">string</span><span class="sxs-lookup"><span data-stu-id="ded1b-128">string</span></span>       | <span data-ttu-id="ded1b-129">テナントの一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="ded1b-129">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="ded1b-130">webId</span><span class="sxs-lookup"><span data-stu-id="ded1b-130">webId</span></span>            | <span data-ttu-id="ded1b-131">string</span><span class="sxs-lookup"><span data-stu-id="ded1b-131">string</span></span>       | <span data-ttu-id="ded1b-132">アイテムのサイト (SPWeb) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="ded1b-132">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="ded1b-133">備考</span><span class="sxs-lookup"><span data-stu-id="ded1b-133">Remarks</span></span>

<span data-ttu-id="ded1b-134">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ded1b-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": []
}
-->
