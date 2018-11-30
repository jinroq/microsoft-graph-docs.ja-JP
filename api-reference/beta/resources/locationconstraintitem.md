---
title: locationConstraintItem リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
ms.openlocfilehash: f29ff1283d876e726e27473485a183956137f981
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066788"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="e1ad3-103">locationConstraintItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1ad3-103">locationConstraintItem resource type</span></span>

> <span data-ttu-id="e1ad3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1ad3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1ad3-106">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-106">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="e1ad3-107">[location](location.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-107">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1ad3-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1ad3-108">JSON representation</span></span>

<span data-ttu-id="e1ad3-109">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e1ad3-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e1ad3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1ad3-110">Properties</span></span>
| <span data-ttu-id="e1ad3-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1ad3-111">Property</span></span>     | <span data-ttu-id="e1ad3-112">型</span><span class="sxs-lookup"><span data-stu-id="e1ad3-112">Type</span></span>   |<span data-ttu-id="e1ad3-113">説明</span><span class="sxs-lookup"><span data-stu-id="e1ad3-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e1ad3-114">address</span><span class="sxs-lookup"><span data-stu-id="e1ad3-114">address</span></span> | [<span data-ttu-id="e1ad3-115">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e1ad3-115">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="e1ad3-116">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-116">The street address of the location.</span></span> |
| <span data-ttu-id="e1ad3-117">coordinates</span><span class="sxs-lookup"><span data-stu-id="e1ad3-117">coordinates</span></span> | [<span data-ttu-id="e1ad3-118">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="e1ad3-118">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="e1ad3-119">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-119">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="e1ad3-120">displayName</span><span class="sxs-lookup"><span data-stu-id="e1ad3-120">displayName</span></span>  | <span data-ttu-id="e1ad3-121">String</span><span class="sxs-lookup"><span data-stu-id="e1ad3-121">String</span></span> | <span data-ttu-id="e1ad3-122">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-122">The name associated with the location.</span></span>                       |
| <span data-ttu-id="e1ad3-123">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e1ad3-123">locationEmailAddress</span></span> | <span data-ttu-id="e1ad3-124">String</span><span class="sxs-lookup"><span data-stu-id="e1ad3-124">String</span></span> | <span data-ttu-id="e1ad3-125">場所のメール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-125">Optional email address of the location.</span></span> |
| <span data-ttu-id="e1ad3-126">locationUri</span><span class="sxs-lookup"><span data-stu-id="e1ad3-126">locationUri</span></span> | <span data-ttu-id="e1ad3-127">String</span><span class="sxs-lookup"><span data-stu-id="e1ad3-127">String</span></span> | <span data-ttu-id="e1ad3-128">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-128">Optional URI representing the location.</span></span> |
| <span data-ttu-id="e1ad3-129">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="e1ad3-129">resolveAvailability</span></span> | <span data-ttu-id="e1ad3-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ad3-130">Boolean</span></span> | <span data-ttu-id="e1ad3-p102">true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user-findmeetingtimes.md) は空いている別のリソースを検索します。false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="e1ad3-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->