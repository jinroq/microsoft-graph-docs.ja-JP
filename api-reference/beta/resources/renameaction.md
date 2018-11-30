---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
ms.openlocfilehash: 12956ab51923f6d9f175b25203bf2921a64a8a6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069811"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="880a6-102">RenameAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="880a6-102">RenameAction resource type</span></span>

> <span data-ttu-id="880a6-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="880a6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="880a6-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="880a6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="880a6-105">[**itemActivity**][activity] に **RenameAction** リソースがある場合、アクティビティがアイテムの名前を変更したことを示します。</span><span class="sxs-lookup"><span data-stu-id="880a6-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="880a6-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="880a6-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="880a6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="880a6-107">Properties</span></span>

| <span data-ttu-id="880a6-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="880a6-108">Property name</span></span> | <span data-ttu-id="880a6-109">型</span><span class="sxs-lookup"><span data-stu-id="880a6-109">Type</span></span>   | <span data-ttu-id="880a6-110">説明</span><span class="sxs-lookup"><span data-stu-id="880a6-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="880a6-111">oldName</span><span class="sxs-lookup"><span data-stu-id="880a6-111">oldName</span></span>       | <span data-ttu-id="880a6-112">文字列</span><span class="sxs-lookup"><span data-stu-id="880a6-112">string</span></span> | <span data-ttu-id="880a6-113">アイテムの変更前の名前。</span><span class="sxs-lookup"><span data-stu-id="880a6-113">The previous name of the item.</span></span>
| <span data-ttu-id="880a6-114">newName</span><span class="sxs-lookup"><span data-stu-id="880a6-114">newName</span></span>       | <span data-ttu-id="880a6-115">文字列</span><span class="sxs-lookup"><span data-stu-id="880a6-115">string</span></span> | <span data-ttu-id="880a6-116">項目の新しい名前です。</span><span class="sxs-lookup"><span data-stu-id="880a6-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="880a6-117">備考</span><span class="sxs-lookup"><span data-stu-id="880a6-117">Remarks</span></span>

<span data-ttu-id="880a6-118">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="880a6-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction"
} -->
