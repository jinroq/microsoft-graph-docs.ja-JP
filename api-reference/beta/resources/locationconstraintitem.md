---
title: locationConstraintItem リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8e0b14096d8be66a6aab6d4e73cf0941d7db7b5c
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057002"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="758ed-103">locationConstraintItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="758ed-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="758ed-104">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="758ed-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="758ed-105">[locationDataModel](locationdatamodel.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="758ed-105">Derived from [locationDataModel](locationdatamodel.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="758ed-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="758ed-106">JSON representation</span></span>

<span data-ttu-id="758ed-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="758ed-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```
## <a name="properties"></a><span data-ttu-id="758ed-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="758ed-108">Properties</span></span>
| <span data-ttu-id="758ed-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="758ed-109">Property</span></span>     | <span data-ttu-id="758ed-110">種類</span><span class="sxs-lookup"><span data-stu-id="758ed-110">Type</span></span>   |<span data-ttu-id="758ed-111">説明</span><span class="sxs-lookup"><span data-stu-id="758ed-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="758ed-112">address</span><span class="sxs-lookup"><span data-stu-id="758ed-112">address</span></span> | [<span data-ttu-id="758ed-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="758ed-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="758ed-114">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="758ed-114">The street address of the location.</span></span> |
| <span data-ttu-id="758ed-115">coordinates</span><span class="sxs-lookup"><span data-stu-id="758ed-115">coordinates</span></span> | [<span data-ttu-id="758ed-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="758ed-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="758ed-117">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="758ed-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="758ed-118">displayName</span><span class="sxs-lookup"><span data-stu-id="758ed-118">displayName</span></span>  | <span data-ttu-id="758ed-119">文字列</span><span class="sxs-lookup"><span data-stu-id="758ed-119">String</span></span> | <span data-ttu-id="758ed-120">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="758ed-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="758ed-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="758ed-121">locationEmailAddress</span></span> | <span data-ttu-id="758ed-122">String</span><span class="sxs-lookup"><span data-stu-id="758ed-122">String</span></span> | <span data-ttu-id="758ed-123">場所のメール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="758ed-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="758ed-124">locationUri</span><span class="sxs-lookup"><span data-stu-id="758ed-124">locationUri</span></span> | <span data-ttu-id="758ed-125">String</span><span class="sxs-lookup"><span data-stu-id="758ed-125">String</span></span> | <span data-ttu-id="758ed-126">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="758ed-126">Optional URI representing the location.</span></span> |
| <span data-ttu-id="758ed-127">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="758ed-127">resolveAvailability</span></span> | <span data-ttu-id="758ed-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="758ed-128">Boolean</span></span> | <span data-ttu-id="758ed-p101">true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user-findmeetingtimes.md) は空いている別のリソースを検索します。false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="758ed-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraintitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
