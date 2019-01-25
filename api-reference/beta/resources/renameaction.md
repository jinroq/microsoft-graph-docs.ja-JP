---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: bc731a94167e16518c8dd9eaea7deabd5f519f7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515469"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="e55b6-102">RenameAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e55b6-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e55b6-103">[**itemActivity**][activity] に **RenameAction** リソースがある場合、アクティビティがアイテムの名前を変更したことを示します。</span><span class="sxs-lookup"><span data-stu-id="e55b6-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e55b6-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e55b6-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e55b6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e55b6-105">Properties</span></span>

| <span data-ttu-id="e55b6-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e55b6-106">Property name</span></span> | <span data-ttu-id="e55b6-107">種類</span><span class="sxs-lookup"><span data-stu-id="e55b6-107">Type</span></span>   | <span data-ttu-id="e55b6-108">説明</span><span class="sxs-lookup"><span data-stu-id="e55b6-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e55b6-109">oldName</span><span class="sxs-lookup"><span data-stu-id="e55b6-109">oldName</span></span>       | <span data-ttu-id="e55b6-110">string</span><span class="sxs-lookup"><span data-stu-id="e55b6-110">string</span></span> | <span data-ttu-id="e55b6-111">アイテムの変更前の名前。</span><span class="sxs-lookup"><span data-stu-id="e55b6-111">The previous name of the item.</span></span>
| <span data-ttu-id="e55b6-112">newname</span><span class="sxs-lookup"><span data-stu-id="e55b6-112">newName</span></span>       | <span data-ttu-id="e55b6-113">string</span><span class="sxs-lookup"><span data-stu-id="e55b6-113">string</span></span> | <span data-ttu-id="e55b6-114">項目の新しい名前です。</span><span class="sxs-lookup"><span data-stu-id="e55b6-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="e55b6-115">備考</span><span class="sxs-lookup"><span data-stu-id="e55b6-115">Remarks</span></span>

<span data-ttu-id="e55b6-116">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="e55b6-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
