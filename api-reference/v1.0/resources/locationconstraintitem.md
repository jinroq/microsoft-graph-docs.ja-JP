---
title: locationConstraintItem リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ee841112aa641069ec64d744120f460713e51c7d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036457"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="66ee3-103">locationConstraintItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66ee3-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="66ee3-104">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="66ee3-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="66ee3-105">[location](location.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="66ee3-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="66ee3-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66ee3-106">JSON representation</span></span>

<span data-ttu-id="66ee3-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="66ee3-107">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="66ee3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66ee3-108">Properties</span></span>
| <span data-ttu-id="66ee3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66ee3-109">Property</span></span>     | <span data-ttu-id="66ee3-110">型</span><span class="sxs-lookup"><span data-stu-id="66ee3-110">Type</span></span>   |<span data-ttu-id="66ee3-111">説明</span><span class="sxs-lookup"><span data-stu-id="66ee3-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66ee3-112">address</span><span class="sxs-lookup"><span data-stu-id="66ee3-112">address</span></span> | [<span data-ttu-id="66ee3-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="66ee3-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="66ee3-114">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="66ee3-114">The street address of the location.</span></span> |
| <span data-ttu-id="66ee3-115">displayName</span><span class="sxs-lookup"><span data-stu-id="66ee3-115">displayName</span></span>  | <span data-ttu-id="66ee3-116">String</span><span class="sxs-lookup"><span data-stu-id="66ee3-116">String</span></span> | <span data-ttu-id="66ee3-117">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="66ee3-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="66ee3-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="66ee3-118">locationEmailAddress</span></span> | <span data-ttu-id="66ee3-119">String</span><span class="sxs-lookup"><span data-stu-id="66ee3-119">String</span></span> | <span data-ttu-id="66ee3-120">場所の電子メール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="66ee3-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="66ee3-121">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="66ee3-121">resolveAvailability</span></span> | <span data-ttu-id="66ee3-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="66ee3-122">Boolean</span></span> | <span data-ttu-id="66ee3-p101">true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user-findmeetingtimes.md) は空いている別のリソースを検索します。false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="66ee3-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
