---
title: locationConstraintItem リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7063eb0a7aa437b51a2bfecb482012771297f766
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936256"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="979fa-103">locationConstraintItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="979fa-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="979fa-104">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="979fa-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="979fa-105">[location](location.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="979fa-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="979fa-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="979fa-106">JSON representation</span></span>

<span data-ttu-id="979fa-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="979fa-107">Here is a JSON representation of the resource</span></span>

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
  "locationType": "string",
  "locationUri": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="979fa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="979fa-108">Properties</span></span>
| <span data-ttu-id="979fa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="979fa-109">Property</span></span>     | <span data-ttu-id="979fa-110">型</span><span class="sxs-lookup"><span data-stu-id="979fa-110">Type</span></span>   |<span data-ttu-id="979fa-111">説明</span><span class="sxs-lookup"><span data-stu-id="979fa-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="979fa-112">address</span><span class="sxs-lookup"><span data-stu-id="979fa-112">address</span></span> | [<span data-ttu-id="979fa-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="979fa-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="979fa-114">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="979fa-114">The street address of the location.</span></span> |
| <span data-ttu-id="979fa-115">coordinates</span><span class="sxs-lookup"><span data-stu-id="979fa-115">coordinates</span></span> | [<span data-ttu-id="979fa-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="979fa-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="979fa-117">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="979fa-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="979fa-118">displayName</span><span class="sxs-lookup"><span data-stu-id="979fa-118">displayName</span></span>  | <span data-ttu-id="979fa-119">String</span><span class="sxs-lookup"><span data-stu-id="979fa-119">String</span></span> | <span data-ttu-id="979fa-120">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="979fa-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="979fa-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="979fa-121">locationEmailAddress</span></span> | <span data-ttu-id="979fa-122">String</span><span class="sxs-lookup"><span data-stu-id="979fa-122">String</span></span> | <span data-ttu-id="979fa-123">場所の電子メール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="979fa-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="979fa-124">locationType</span><span class="sxs-lookup"><span data-stu-id="979fa-124">locationType</span></span> | <span data-ttu-id="979fa-125">locationType</span><span class="sxs-lookup"><span data-stu-id="979fa-125">locationType</span></span> | <span data-ttu-id="979fa-126">場所の種類。</span><span class="sxs-lookup"><span data-stu-id="979fa-126">The type of location.</span></span> <span data-ttu-id="979fa-127">可能な値は、`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress` です。</span><span class="sxs-lookup"><span data-stu-id="979fa-127">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="979fa-128">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="979fa-128">Read-only.</span></span>|
| <span data-ttu-id="979fa-129">locationUri</span><span class="sxs-lookup"><span data-stu-id="979fa-129">locationUri</span></span> | <span data-ttu-id="979fa-130">String</span><span class="sxs-lookup"><span data-stu-id="979fa-130">String</span></span> | <span data-ttu-id="979fa-131">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="979fa-131">Optional URI representing the location.</span></span> |
| <span data-ttu-id="979fa-132">resolveavailability</span><span class="sxs-lookup"><span data-stu-id="979fa-132">resolveAvailability</span></span> | <span data-ttu-id="979fa-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="979fa-133">Boolean</span></span> | <span data-ttu-id="979fa-p102">true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user-findmeetingtimes.md) は空いている別のリソースを検索します。false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="979fa-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="979fa-137">uniqueId</span><span class="sxs-lookup"><span data-stu-id="979fa-137">uniqueId</span></span> | <span data-ttu-id="979fa-138">String</span><span class="sxs-lookup"><span data-stu-id="979fa-138">String</span></span> | <span data-ttu-id="979fa-139">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="979fa-139">For internal use only.</span></span>|
| <span data-ttu-id="979fa-140">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="979fa-140">uniqueIdType</span></span> | <span data-ttu-id="979fa-141">String</span><span class="sxs-lookup"><span data-stu-id="979fa-141">String</span></span> | <span data-ttu-id="979fa-142">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="979fa-142">For internal use only.</span></span> |

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
