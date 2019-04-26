---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: aa20816165ed4f41e8b89af106e3f781b1be8dd7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562602"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="a37e7-102">MoveAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a37e7-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a37e7-103">[**itemActivity**][activity] に **MoveAction** リソースがある場合、アクティビティがアイテムを移動したことを示します。</span><span class="sxs-lookup"><span data-stu-id="a37e7-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="a37e7-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a37e7-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a37e7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a37e7-105">Properties</span></span>

| <span data-ttu-id="a37e7-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a37e7-106">Property name</span></span> | <span data-ttu-id="a37e7-107">種類</span><span class="sxs-lookup"><span data-stu-id="a37e7-107">Type</span></span>   | <span data-ttu-id="a37e7-108">説明</span><span class="sxs-lookup"><span data-stu-id="a37e7-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a37e7-109">from</span><span class="sxs-lookup"><span data-stu-id="a37e7-109">from</span></span>          | <span data-ttu-id="a37e7-110">string</span><span class="sxs-lookup"><span data-stu-id="a37e7-110">string</span></span> | <span data-ttu-id="a37e7-111">アイテムの移動元の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="a37e7-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="a37e7-112">to</span><span class="sxs-lookup"><span data-stu-id="a37e7-112">to</span></span>            | <span data-ttu-id="a37e7-113">string</span><span class="sxs-lookup"><span data-stu-id="a37e7-113">string</span></span> | <span data-ttu-id="a37e7-114">アイテムの移動先の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="a37e7-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="a37e7-115">備考</span><span class="sxs-lookup"><span data-stu-id="a37e7-115">Remarks</span></span>

<span data-ttu-id="a37e7-116">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="a37e7-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/moveaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
