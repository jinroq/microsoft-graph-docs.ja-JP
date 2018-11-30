---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
ms.openlocfilehash: 6cf2e574ea6d2a5cf5344dcf4d7ef5532a6a5b16
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069799"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="50701-102">SharePointIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50701-102">SharePointIds resource type</span></span>

> <span data-ttu-id="50701-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="50701-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50701-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50701-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50701-105">**SharePointIds** リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="50701-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="50701-106">**注:** 個人用の OneDrive から返されたアイテムには **SharePointIds** ファセットは含まれません。</span><span class="sxs-lookup"><span data-stu-id="50701-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50701-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50701-107">JSON representation</span></span>

<span data-ttu-id="50701-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="50701-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="50701-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50701-109">Properties</span></span>

| <span data-ttu-id="50701-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50701-110">Property</span></span>         | <span data-ttu-id="50701-111">型</span><span class="sxs-lookup"><span data-stu-id="50701-111">Type</span></span>         | <span data-ttu-id="50701-112">説明</span><span class="sxs-lookup"><span data-stu-id="50701-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="50701-113">listId</span><span class="sxs-lookup"><span data-stu-id="50701-113">listId</span></span>           | <span data-ttu-id="50701-114">文字列</span><span class="sxs-lookup"><span data-stu-id="50701-114">string</span></span>       | <span data-ttu-id="50701-115">SharePoint 内にあるアイテムの一覧の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="50701-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="50701-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="50701-116">listItemId</span></span>       | <span data-ttu-id="50701-117">文字列</span><span class="sxs-lookup"><span data-stu-id="50701-117">string</span></span>       | <span data-ttu-id="50701-118">含まれているリスト内にあるアイテムの整数の識別子。</span><span class="sxs-lookup"><span data-stu-id="50701-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="50701-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="50701-119">listItemUniqueId</span></span> | <span data-ttu-id="50701-120">文字列</span><span class="sxs-lookup"><span data-stu-id="50701-120">string</span></span>       | <span data-ttu-id="50701-121">OneDrive for Business または SharePoint サイト内のアイテムの一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="50701-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="50701-122">siteId</span><span class="sxs-lookup"><span data-stu-id="50701-122">siteId</span></span>           | <span data-ttu-id="50701-123">文字列</span><span class="sxs-lookup"><span data-stu-id="50701-123">string</span></span>       | <span data-ttu-id="50701-124">アイテムのサイト コレクション (SPSite) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="50701-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="50701-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="50701-125">siteUrl</span></span>          | <span data-ttu-id="50701-126">string (URL)</span><span class="sxs-lookup"><span data-stu-id="50701-126">string (url)</span></span> | <span data-ttu-id="50701-127">アイテムが含まれるサイトの SharePoint URL です。</span><span class="sxs-lookup"><span data-stu-id="50701-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="50701-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="50701-128">tenantId</span></span>         | <span data-ttu-id="50701-129">文字列</span><span class="sxs-lookup"><span data-stu-id="50701-129">string</span></span>       | <span data-ttu-id="50701-130">借用地の一意の識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="50701-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="50701-131">webId</span><span class="sxs-lookup"><span data-stu-id="50701-131">webId</span></span>            | <span data-ttu-id="50701-132">文字列</span><span class="sxs-lookup"><span data-stu-id="50701-132">string</span></span>       | <span data-ttu-id="50701-133">アイテムのサイト (SPWeb) の一意識別子 (guid)。</span><span class="sxs-lookup"><span data-stu-id="50701-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="50701-134">備考</span><span class="sxs-lookup"><span data-stu-id="50701-134">Remarks</span></span>

<span data-ttu-id="50701-135">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50701-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
