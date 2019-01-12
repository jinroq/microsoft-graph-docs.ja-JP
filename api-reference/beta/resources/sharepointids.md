---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 641b4f5b8d78a38324b7b19c9136e8a53532a9d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979937"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="d305c-102">SharePointIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d305c-102">SharePointIds resource type</span></span>

> <span data-ttu-id="d305c-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d305c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d305c-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d305c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d305c-105">**SharePointIds** リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="d305c-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="d305c-106">**注:** 個人用の OneDrive から返されたアイテムには **SharePointIds** ファセットは含まれません。</span><span class="sxs-lookup"><span data-stu-id="d305c-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d305c-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d305c-107">JSON representation</span></span>

<span data-ttu-id="d305c-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d305c-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d305c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d305c-109">Properties</span></span>

| <span data-ttu-id="d305c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d305c-110">Property</span></span>         | <span data-ttu-id="d305c-111">種類</span><span class="sxs-lookup"><span data-stu-id="d305c-111">Type</span></span>         | <span data-ttu-id="d305c-112">説明</span><span class="sxs-lookup"><span data-stu-id="d305c-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="d305c-113">listId</span><span class="sxs-lookup"><span data-stu-id="d305c-113">listId</span></span>           | <span data-ttu-id="d305c-114">文字列</span><span class="sxs-lookup"><span data-stu-id="d305c-114">string</span></span>       | <span data-ttu-id="d305c-115">SharePoint 内にあるアイテムの一覧の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="d305c-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="d305c-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="d305c-116">listItemId</span></span>       | <span data-ttu-id="d305c-117">文字列</span><span class="sxs-lookup"><span data-stu-id="d305c-117">string</span></span>       | <span data-ttu-id="d305c-118">含まれているリスト内にあるアイテムの整数の識別子。</span><span class="sxs-lookup"><span data-stu-id="d305c-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="d305c-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="d305c-119">listItemUniqueId</span></span> | <span data-ttu-id="d305c-120">文字列</span><span class="sxs-lookup"><span data-stu-id="d305c-120">string</span></span>       | <span data-ttu-id="d305c-121">OneDrive for Business または SharePoint サイト内のアイテムの一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="d305c-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="d305c-122">siteId</span><span class="sxs-lookup"><span data-stu-id="d305c-122">siteId</span></span>           | <span data-ttu-id="d305c-123">文字列</span><span class="sxs-lookup"><span data-stu-id="d305c-123">string</span></span>       | <span data-ttu-id="d305c-124">アイテムのサイト コレクション (SPSite) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="d305c-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="d305c-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="d305c-125">siteUrl</span></span>          | <span data-ttu-id="d305c-126">string (URL)</span><span class="sxs-lookup"><span data-stu-id="d305c-126">string (url)</span></span> | <span data-ttu-id="d305c-127">アイテムが含まれるサイトの SharePoint URL です。</span><span class="sxs-lookup"><span data-stu-id="d305c-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="d305c-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="d305c-128">tenantId</span></span>         | <span data-ttu-id="d305c-129">文字列</span><span class="sxs-lookup"><span data-stu-id="d305c-129">string</span></span>       | <span data-ttu-id="d305c-130">借用地の一意の識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="d305c-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="d305c-131">webId</span><span class="sxs-lookup"><span data-stu-id="d305c-131">webId</span></span>            | <span data-ttu-id="d305c-132">文字列</span><span class="sxs-lookup"><span data-stu-id="d305c-132">string</span></span>       | <span data-ttu-id="d305c-133">アイテムのサイト (SPWeb) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="d305c-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="d305c-134">備考</span><span class="sxs-lookup"><span data-stu-id="d305c-134">Remarks</span></span>

<span data-ttu-id="d305c-135">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d305c-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
