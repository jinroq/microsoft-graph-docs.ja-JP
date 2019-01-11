---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: 88fa2738c014f028ebd2cc6e37f83151c7fc984a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835708"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="2e382-102">RenameAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e382-102">RenameAction resource type</span></span>

> <span data-ttu-id="2e382-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2e382-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e382-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e382-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e382-105">[**itemActivity**][activity] に **RenameAction** リソースがある場合、アクティビティがアイテムの名前を変更したことを示します。</span><span class="sxs-lookup"><span data-stu-id="2e382-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="2e382-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e382-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

## <a name="properties"></a><span data-ttu-id="2e382-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e382-107">Properties</span></span>

| <span data-ttu-id="2e382-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2e382-108">Property name</span></span> | <span data-ttu-id="2e382-109">Type</span><span class="sxs-lookup"><span data-stu-id="2e382-109">Type</span></span>   | <span data-ttu-id="2e382-110">説明</span><span class="sxs-lookup"><span data-stu-id="2e382-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2e382-111">oldName</span><span class="sxs-lookup"><span data-stu-id="2e382-111">oldName</span></span>       | <span data-ttu-id="2e382-112">文字列</span><span class="sxs-lookup"><span data-stu-id="2e382-112">string</span></span> | <span data-ttu-id="2e382-113">アイテムの変更前の名前。</span><span class="sxs-lookup"><span data-stu-id="2e382-113">The previous name of the item.</span></span>
| <span data-ttu-id="2e382-114">newName</span><span class="sxs-lookup"><span data-stu-id="2e382-114">newName</span></span>       | <span data-ttu-id="2e382-115">文字列</span><span class="sxs-lookup"><span data-stu-id="2e382-115">string</span></span> | <span data-ttu-id="2e382-116">項目の新しい名前です。</span><span class="sxs-lookup"><span data-stu-id="2e382-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="2e382-117">備考</span><span class="sxs-lookup"><span data-stu-id="2e382-117">Remarks</span></span>

<span data-ttu-id="2e382-118">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="2e382-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction"
} -->
