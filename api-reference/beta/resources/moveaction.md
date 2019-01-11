---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 40049b506c72af5aacddf461b22e1ddd280d7ad4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852900"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="0bd21-102">MoveAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0bd21-102">MoveAction resource type</span></span>

> <span data-ttu-id="0bd21-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0bd21-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bd21-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bd21-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0bd21-105">[**itemActivity**][activity] に **MoveAction** リソースがある場合、アクティビティがアイテムを移動したことを示します。</span><span class="sxs-lookup"><span data-stu-id="0bd21-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0bd21-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0bd21-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0bd21-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bd21-107">Properties</span></span>

| <span data-ttu-id="0bd21-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0bd21-108">Property name</span></span> | <span data-ttu-id="0bd21-109">Type</span><span class="sxs-lookup"><span data-stu-id="0bd21-109">Type</span></span>   | <span data-ttu-id="0bd21-110">説明</span><span class="sxs-lookup"><span data-stu-id="0bd21-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="0bd21-111">from</span><span class="sxs-lookup"><span data-stu-id="0bd21-111">from</span></span>          | <span data-ttu-id="0bd21-112">文字列</span><span class="sxs-lookup"><span data-stu-id="0bd21-112">string</span></span> | <span data-ttu-id="0bd21-113">アイテムの移動元の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="0bd21-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="0bd21-114">to</span><span class="sxs-lookup"><span data-stu-id="0bd21-114">to</span></span>            | <span data-ttu-id="0bd21-115">文字列</span><span class="sxs-lookup"><span data-stu-id="0bd21-115">string</span></span> | <span data-ttu-id="0bd21-116">アイテムの移動先の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="0bd21-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="0bd21-117">備考</span><span class="sxs-lookup"><span data-stu-id="0bd21-117">Remarks</span></span>

<span data-ttu-id="0bd21-118">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="0bd21-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction"
} -->
