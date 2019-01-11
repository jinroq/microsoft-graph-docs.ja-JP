---
title: locationConstraintItem リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
ms.openlocfilehash: 4c44a97a3ed0d5bcf56204fab1527c7e4b58455d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874083"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="6970e-103">locationConstraintItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6970e-103">locationConstraintItem resource type</span></span>

> <span data-ttu-id="6970e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6970e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6970e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6970e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6970e-106">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="6970e-106">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="6970e-107">[location](location.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="6970e-107">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6970e-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6970e-108">JSON representation</span></span>

<span data-ttu-id="6970e-109">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6970e-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6970e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6970e-110">Properties</span></span>
| <span data-ttu-id="6970e-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6970e-111">Property</span></span>     | <span data-ttu-id="6970e-112">種類</span><span class="sxs-lookup"><span data-stu-id="6970e-112">Type</span></span>   |<span data-ttu-id="6970e-113">説明</span><span class="sxs-lookup"><span data-stu-id="6970e-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6970e-114">address</span><span class="sxs-lookup"><span data-stu-id="6970e-114">address</span></span> | [<span data-ttu-id="6970e-115">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6970e-115">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="6970e-116">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="6970e-116">The street address of the location.</span></span> |
| <span data-ttu-id="6970e-117">coordinates</span><span class="sxs-lookup"><span data-stu-id="6970e-117">coordinates</span></span> | [<span data-ttu-id="6970e-118">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="6970e-118">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="6970e-119">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="6970e-119">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="6970e-120">displayName</span><span class="sxs-lookup"><span data-stu-id="6970e-120">displayName</span></span>  | <span data-ttu-id="6970e-121">String</span><span class="sxs-lookup"><span data-stu-id="6970e-121">String</span></span> | <span data-ttu-id="6970e-122">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="6970e-122">The name associated with the location.</span></span>                       |
| <span data-ttu-id="6970e-123">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="6970e-123">locationEmailAddress</span></span> | <span data-ttu-id="6970e-124">String</span><span class="sxs-lookup"><span data-stu-id="6970e-124">String</span></span> | <span data-ttu-id="6970e-125">場所のメール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="6970e-125">Optional email address of the location.</span></span> |
| <span data-ttu-id="6970e-126">locationUri</span><span class="sxs-lookup"><span data-stu-id="6970e-126">locationUri</span></span> | <span data-ttu-id="6970e-127">String</span><span class="sxs-lookup"><span data-stu-id="6970e-127">String</span></span> | <span data-ttu-id="6970e-128">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="6970e-128">Optional URI representing the location.</span></span> |
| <span data-ttu-id="6970e-129">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="6970e-129">resolveAvailability</span></span> | <span data-ttu-id="6970e-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="6970e-130">Boolean</span></span> | <span data-ttu-id="6970e-p102">true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user-findmeetingtimes.md) は空いている別のリソースを検索します。false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="6970e-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
