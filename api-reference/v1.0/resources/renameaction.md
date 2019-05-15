---
author: daspek
ms.author: dspektor
title: renameAction リソースの種類
description: RenameAction オブジェクトは、アイテムの名前を変更したアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bce040130d74b7977fc1f988a34edde674f9e0d4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970763"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="14281-103">renameAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14281-103">renameAction resource type</span></span>

<span data-ttu-id="14281-104">[**Itemactivity**] [ activity]に**renameaction**リソースが存在することは、アクティビティがアイテムの名前を変更したことを示します。</span><span class="sxs-lookup"><span data-stu-id="14281-104">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="14281-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="14281-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="14281-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14281-106">Properties</span></span>

| <span data-ttu-id="14281-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="14281-107">Property name</span></span> | <span data-ttu-id="14281-108">種類</span><span class="sxs-lookup"><span data-stu-id="14281-108">Type</span></span>   | <span data-ttu-id="14281-109">説明</span><span class="sxs-lookup"><span data-stu-id="14281-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="14281-110">oldName</span><span class="sxs-lookup"><span data-stu-id="14281-110">oldName</span></span>       | <span data-ttu-id="14281-111">string</span><span class="sxs-lookup"><span data-stu-id="14281-111">string</span></span> | <span data-ttu-id="14281-112">アイテムの変更前の名前。</span><span class="sxs-lookup"><span data-stu-id="14281-112">The previous name of the item.</span></span>
| <span data-ttu-id="14281-113">newName</span><span class="sxs-lookup"><span data-stu-id="14281-113">newName</span></span>       | <span data-ttu-id="14281-114">string</span><span class="sxs-lookup"><span data-stu-id="14281-114">string</span></span> | <span data-ttu-id="14281-115">アイテムの新しい名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="14281-115">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14281-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14281-116">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->
