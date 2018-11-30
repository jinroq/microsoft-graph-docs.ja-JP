---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
ms.openlocfilehash: 28788090ccda113d6f4cd669e89777be84e6c2d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022416"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="7429a-102">SharePointIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7429a-102">SharePointIds resource type</span></span>

<span data-ttu-id="7429a-103">**SharePointIds** リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="7429a-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="7429a-104">**注:** 個人用の OneDrive から返されたアイテムには **SharePointIds** ファセットは含まれません。</span><span class="sxs-lookup"><span data-stu-id="7429a-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7429a-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7429a-105">JSON representation</span></span>

<span data-ttu-id="7429a-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7429a-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7429a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7429a-107">Properties</span></span>

| <span data-ttu-id="7429a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7429a-108">Property</span></span>         | <span data-ttu-id="7429a-109">型</span><span class="sxs-lookup"><span data-stu-id="7429a-109">Type</span></span>         | <span data-ttu-id="7429a-110">説明</span><span class="sxs-lookup"><span data-stu-id="7429a-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="7429a-111">listId</span><span class="sxs-lookup"><span data-stu-id="7429a-111">listId</span></span>           | <span data-ttu-id="7429a-112">string</span><span class="sxs-lookup"><span data-stu-id="7429a-112">string</span></span>       | <span data-ttu-id="7429a-113">SharePoint 内にあるアイテムの一覧の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="7429a-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="7429a-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="7429a-114">listItemId</span></span>       | <span data-ttu-id="7429a-115">string</span><span class="sxs-lookup"><span data-stu-id="7429a-115">string</span></span>       | <span data-ttu-id="7429a-116">含まれているリスト内にあるアイテムの整数の識別子。</span><span class="sxs-lookup"><span data-stu-id="7429a-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="7429a-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="7429a-117">listItemUniqueId</span></span> | <span data-ttu-id="7429a-118">string</span><span class="sxs-lookup"><span data-stu-id="7429a-118">string</span></span>       | <span data-ttu-id="7429a-119">OneDrive for Business または SharePoint サイト内のアイテムの一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="7429a-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="7429a-120">siteId</span><span class="sxs-lookup"><span data-stu-id="7429a-120">siteId</span></span>           | <span data-ttu-id="7429a-121">string</span><span class="sxs-lookup"><span data-stu-id="7429a-121">string</span></span>       | <span data-ttu-id="7429a-122">アイテムのサイト コレクション (SPSite) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="7429a-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="7429a-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="7429a-123">siteUrl</span></span>          | <span data-ttu-id="7429a-124">string (URL)</span><span class="sxs-lookup"><span data-stu-id="7429a-124">string (url)</span></span> | <span data-ttu-id="7429a-125">アイテムが含まれるサイトの SharePoint URL です。</span><span class="sxs-lookup"><span data-stu-id="7429a-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="7429a-126">webId</span><span class="sxs-lookup"><span data-stu-id="7429a-126">webId</span></span>            | <span data-ttu-id="7429a-127">string</span><span class="sxs-lookup"><span data-stu-id="7429a-127">string</span></span>       | <span data-ttu-id="7429a-128">アイテムのサイト (SPWeb) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="7429a-128">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="7429a-129">備考</span><span class="sxs-lookup"><span data-stu-id="7429a-129">Remarks</span></span>

<span data-ttu-id="7429a-130">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7429a-130">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
