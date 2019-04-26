---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: bc731a94167e16518c8dd9eaea7deabd5f519f7b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563110"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="f15b9-102">RenameAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f15b9-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f15b9-103">[**itemActivity**][activity] に **RenameAction** リソースがある場合、アクティビティがアイテムの名前を変更したことを示します。</span><span class="sxs-lookup"><span data-stu-id="f15b9-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f15b9-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f15b9-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f15b9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f15b9-105">Properties</span></span>

| <span data-ttu-id="f15b9-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f15b9-106">Property name</span></span> | <span data-ttu-id="f15b9-107">種類</span><span class="sxs-lookup"><span data-stu-id="f15b9-107">Type</span></span>   | <span data-ttu-id="f15b9-108">説明</span><span class="sxs-lookup"><span data-stu-id="f15b9-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f15b9-109">oldName</span><span class="sxs-lookup"><span data-stu-id="f15b9-109">oldName</span></span>       | <span data-ttu-id="f15b9-110">string</span><span class="sxs-lookup"><span data-stu-id="f15b9-110">string</span></span> | <span data-ttu-id="f15b9-111">アイテムの変更前の名前。</span><span class="sxs-lookup"><span data-stu-id="f15b9-111">The previous name of the item.</span></span>
| <span data-ttu-id="f15b9-112">newName</span><span class="sxs-lookup"><span data-stu-id="f15b9-112">newName</span></span>       | <span data-ttu-id="f15b9-113">string</span><span class="sxs-lookup"><span data-stu-id="f15b9-113">string</span></span> | <span data-ttu-id="f15b9-114">アイテムの新しい名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="f15b9-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="f15b9-115">備考</span><span class="sxs-lookup"><span data-stu-id="f15b9-115">Remarks</span></span>

<span data-ttu-id="f15b9-116">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="f15b9-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/renameaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
