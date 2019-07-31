---
author: daspek
description: itemActivity に MoveAction リソースがある場合、アクティビティがアイテムを移動したことを示します。
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9fbb19097b6a1401bd3c0b6dba4ce1fd5649e706
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009644"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="8b0c1-103">MoveAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b0c1-103">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b0c1-104">[**itemActivity**][activity] に **MoveAction** リソースがある場合、アクティビティがアイテムを移動したことを示します。</span><span class="sxs-lookup"><span data-stu-id="8b0c1-104">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8b0c1-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b0c1-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8b0c1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b0c1-106">Properties</span></span>

| <span data-ttu-id="8b0c1-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8b0c1-107">Property name</span></span> | <span data-ttu-id="8b0c1-108">種類</span><span class="sxs-lookup"><span data-stu-id="8b0c1-108">Type</span></span>   | <span data-ttu-id="8b0c1-109">説明</span><span class="sxs-lookup"><span data-stu-id="8b0c1-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8b0c1-110">from</span><span class="sxs-lookup"><span data-stu-id="8b0c1-110">from</span></span>          | <span data-ttu-id="8b0c1-111">string</span><span class="sxs-lookup"><span data-stu-id="8b0c1-111">string</span></span> | <span data-ttu-id="8b0c1-112">アイテムの移動元の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="8b0c1-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="8b0c1-113">to</span><span class="sxs-lookup"><span data-stu-id="8b0c1-113">to</span></span>            | <span data-ttu-id="8b0c1-114">string</span><span class="sxs-lookup"><span data-stu-id="8b0c1-114">string</span></span> | <span data-ttu-id="8b0c1-115">アイテムの移動先の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="8b0c1-115">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="8b0c1-116">備考</span><span class="sxs-lookup"><span data-stu-id="8b0c1-116">Remarks</span></span>

<span data-ttu-id="8b0c1-117">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="8b0c1-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
