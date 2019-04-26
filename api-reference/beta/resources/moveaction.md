---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 0715f8e9743c4384e8fbd851fe88563e9eaf9666
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342222"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="e1414-102">MoveAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1414-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1414-103">[**itemActivity**][activity] に **MoveAction** リソースがある場合、アクティビティがアイテムを移動したことを示します。</span><span class="sxs-lookup"><span data-stu-id="e1414-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e1414-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1414-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e1414-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1414-105">Properties</span></span>

| <span data-ttu-id="e1414-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e1414-106">Property name</span></span> | <span data-ttu-id="e1414-107">種類</span><span class="sxs-lookup"><span data-stu-id="e1414-107">Type</span></span>   | <span data-ttu-id="e1414-108">説明</span><span class="sxs-lookup"><span data-stu-id="e1414-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e1414-109">from</span><span class="sxs-lookup"><span data-stu-id="e1414-109">from</span></span>          | <span data-ttu-id="e1414-110">string</span><span class="sxs-lookup"><span data-stu-id="e1414-110">string</span></span> | <span data-ttu-id="e1414-111">アイテムの移動元の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="e1414-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="e1414-112">to</span><span class="sxs-lookup"><span data-stu-id="e1414-112">to</span></span>            | <span data-ttu-id="e1414-113">string</span><span class="sxs-lookup"><span data-stu-id="e1414-113">string</span></span> | <span data-ttu-id="e1414-114">アイテムの移動先の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="e1414-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="e1414-115">備考</span><span class="sxs-lookup"><span data-stu-id="e1414-115">Remarks</span></span>

<span data-ttu-id="e1414-116">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="e1414-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
