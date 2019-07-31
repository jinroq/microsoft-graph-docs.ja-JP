---
author: daspek
description: itemActivity に RenameAction リソースがある場合、アクティビティがアイテムの名前を変更したことを示します。
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d62d3f7f836ece716bdc3e616e1943de8c040652
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965423"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="3b96d-103">RenameAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b96d-103">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b96d-104">[**itemActivity**][activity] に **RenameAction** リソースがある場合、アクティビティがアイテムの名前を変更したことを示します。</span><span class="sxs-lookup"><span data-stu-id="3b96d-104">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="3b96d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b96d-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3b96d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b96d-106">Properties</span></span>

| <span data-ttu-id="3b96d-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="3b96d-107">Property name</span></span> | <span data-ttu-id="3b96d-108">種類</span><span class="sxs-lookup"><span data-stu-id="3b96d-108">Type</span></span>   | <span data-ttu-id="3b96d-109">説明</span><span class="sxs-lookup"><span data-stu-id="3b96d-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="3b96d-110">oldName</span><span class="sxs-lookup"><span data-stu-id="3b96d-110">oldName</span></span>       | <span data-ttu-id="3b96d-111">string</span><span class="sxs-lookup"><span data-stu-id="3b96d-111">string</span></span> | <span data-ttu-id="3b96d-112">アイテムの変更前の名前。</span><span class="sxs-lookup"><span data-stu-id="3b96d-112">The previous name of the item.</span></span>
| <span data-ttu-id="3b96d-113">newName</span><span class="sxs-lookup"><span data-stu-id="3b96d-113">newName</span></span>       | <span data-ttu-id="3b96d-114">string</span><span class="sxs-lookup"><span data-stu-id="3b96d-114">string</span></span> | <span data-ttu-id="3b96d-115">アイテムの新しい名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3b96d-115">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="3b96d-116">備考</span><span class="sxs-lookup"><span data-stu-id="3b96d-116">Remarks</span></span>

<span data-ttu-id="3b96d-117">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="3b96d-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": []
}
-->
