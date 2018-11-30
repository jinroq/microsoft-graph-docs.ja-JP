---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
ms.openlocfilehash: d31cfc9a45b83f74058073ca18ca2df15a9914ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067255"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="2b4d4-102">MoveAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b4d4-102">MoveAction resource type</span></span>

> <span data-ttu-id="2b4d4-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b4d4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b4d4-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b4d4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b4d4-105">[**itemActivity**][activity] に **MoveAction** リソースがある場合、アクティビティがアイテムを移動したことを示します。</span><span class="sxs-lookup"><span data-stu-id="2b4d4-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="2b4d4-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b4d4-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2b4d4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b4d4-107">Properties</span></span>

| <span data-ttu-id="2b4d4-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2b4d4-108">Property name</span></span> | <span data-ttu-id="2b4d4-109">型</span><span class="sxs-lookup"><span data-stu-id="2b4d4-109">Type</span></span>   | <span data-ttu-id="2b4d4-110">説明</span><span class="sxs-lookup"><span data-stu-id="2b4d4-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2b4d4-111">from</span><span class="sxs-lookup"><span data-stu-id="2b4d4-111">from</span></span>          | <span data-ttu-id="2b4d4-112">文字列</span><span class="sxs-lookup"><span data-stu-id="2b4d4-112">string</span></span> | <span data-ttu-id="2b4d4-113">アイテムの移動元の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="2b4d4-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="2b4d4-114">to</span><span class="sxs-lookup"><span data-stu-id="2b4d4-114">to</span></span>            | <span data-ttu-id="2b4d4-115">文字列</span><span class="sxs-lookup"><span data-stu-id="2b4d4-115">string</span></span> | <span data-ttu-id="2b4d4-116">アイテムの移動先の場所の名前。</span><span class="sxs-lookup"><span data-stu-id="2b4d4-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="2b4d4-117">備考</span><span class="sxs-lookup"><span data-stu-id="2b4d4-117">Remarks</span></span>

<span data-ttu-id="2b4d4-118">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="2b4d4-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction"
} -->
