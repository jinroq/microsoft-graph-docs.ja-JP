---
author: daspek
ms.author: dspektor
title: moveAction リソースの種類
description: MoveAction オブジェクトは、アイテムを移動したアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 525558d040109e637e2f3532d16c308a197e45fb
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970777"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="a00d7-103">moveAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a00d7-103">moveAction resource type</span></span>

<span data-ttu-id="a00d7-104">[**Itemactivity**] [ activity]に**moveaction**リソースが存在することは、アクティビティがアイテムを移動したことを示します。</span><span class="sxs-lookup"><span data-stu-id="a00d7-104">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="a00d7-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="a00d7-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="a00d7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a00d7-106">Properties</span></span>

| <span data-ttu-id="a00d7-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a00d7-107">Property name</span></span> | <span data-ttu-id="a00d7-108">種類</span><span class="sxs-lookup"><span data-stu-id="a00d7-108">Type</span></span>   | <span data-ttu-id="a00d7-109">説明</span><span class="sxs-lookup"><span data-stu-id="a00d7-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a00d7-110">from</span><span class="sxs-lookup"><span data-stu-id="a00d7-110">from</span></span>          | <span data-ttu-id="a00d7-111">string</span><span class="sxs-lookup"><span data-stu-id="a00d7-111">string</span></span> | <span data-ttu-id="a00d7-112">アイテムの移動元の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="a00d7-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="a00d7-113">to</span><span class="sxs-lookup"><span data-stu-id="a00d7-113">to</span></span>            | <span data-ttu-id="a00d7-114">string</span><span class="sxs-lookup"><span data-stu-id="a00d7-114">string</span></span> | <span data-ttu-id="a00d7-115">アイテムの移動先の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="a00d7-115">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a00d7-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a00d7-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
