---
title: locationConstraintItem リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d7202f5ba52b1d3331c954e4c6a937d9bc36ae23
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966985"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="8ebca-103">locationConstraintItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ebca-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ebca-104">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="8ebca-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="8ebca-105">[location](location.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="8ebca-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ebca-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ebca-106">JSON representation</span></span>

<span data-ttu-id="8ebca-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8ebca-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8ebca-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ebca-108">Properties</span></span>
| <span data-ttu-id="8ebca-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ebca-109">Property</span></span>     | <span data-ttu-id="8ebca-110">型</span><span class="sxs-lookup"><span data-stu-id="8ebca-110">Type</span></span>   |<span data-ttu-id="8ebca-111">説明</span><span class="sxs-lookup"><span data-stu-id="8ebca-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ebca-112">address</span><span class="sxs-lookup"><span data-stu-id="8ebca-112">address</span></span> | [<span data-ttu-id="8ebca-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="8ebca-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="8ebca-114">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="8ebca-114">The street address of the location.</span></span> |
| <span data-ttu-id="8ebca-115">coordinates</span><span class="sxs-lookup"><span data-stu-id="8ebca-115">coordinates</span></span> | [<span data-ttu-id="8ebca-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="8ebca-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="8ebca-117">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="8ebca-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="8ebca-118">displayName</span><span class="sxs-lookup"><span data-stu-id="8ebca-118">displayName</span></span>  | <span data-ttu-id="8ebca-119">String</span><span class="sxs-lookup"><span data-stu-id="8ebca-119">String</span></span> | <span data-ttu-id="8ebca-120">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="8ebca-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="8ebca-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8ebca-121">locationEmailAddress</span></span> | <span data-ttu-id="8ebca-122">String</span><span class="sxs-lookup"><span data-stu-id="8ebca-122">String</span></span> | <span data-ttu-id="8ebca-123">場所の電子メール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="8ebca-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="8ebca-124">locationType</span><span class="sxs-lookup"><span data-stu-id="8ebca-124">locationType</span></span> | <span data-ttu-id="8ebca-125">locationType</span><span class="sxs-lookup"><span data-stu-id="8ebca-125">locationType</span></span> | <span data-ttu-id="8ebca-126">場所の種類。</span><span class="sxs-lookup"><span data-stu-id="8ebca-126">The type of location.</span></span> <span data-ttu-id="8ebca-127">可能な値は、`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress` です。</span><span class="sxs-lookup"><span data-stu-id="8ebca-127">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="8ebca-128">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8ebca-128">Read-only.</span></span>|
| <span data-ttu-id="8ebca-129">locationUri</span><span class="sxs-lookup"><span data-stu-id="8ebca-129">locationUri</span></span> | <span data-ttu-id="8ebca-130">String</span><span class="sxs-lookup"><span data-stu-id="8ebca-130">String</span></span> | <span data-ttu-id="8ebca-131">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="8ebca-131">Optional URI representing the location.</span></span> |
| <span data-ttu-id="8ebca-132">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="8ebca-132">resolveAvailability</span></span> | <span data-ttu-id="8ebca-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ebca-133">Boolean</span></span> | <span data-ttu-id="8ebca-p102">true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user-findmeetingtimes.md) は空いている別のリソースを検索します。false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="8ebca-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="8ebca-137">uniqueId</span><span class="sxs-lookup"><span data-stu-id="8ebca-137">uniqueId</span></span> | <span data-ttu-id="8ebca-138">String</span><span class="sxs-lookup"><span data-stu-id="8ebca-138">String</span></span> | <span data-ttu-id="8ebca-139">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="8ebca-139">For internal use only.</span></span>|
| <span data-ttu-id="8ebca-140">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="8ebca-140">uniqueIdType</span></span> | <span data-ttu-id="8ebca-141">String</span><span class="sxs-lookup"><span data-stu-id="8ebca-141">String</span></span> | <span data-ttu-id="8ebca-142">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="8ebca-142">For internal use only.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
