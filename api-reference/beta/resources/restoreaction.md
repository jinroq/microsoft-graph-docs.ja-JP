---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
ms.openlocfilehash: f04f9811cefba60d0b06b99605774fb8fbfa0125
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514076"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="9133d-102">RestoreAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9133d-102">RestoreAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9133d-103">[**itemActivity**][activity] に **RestoreAction** リソースがある場合、アクティビティがアイテムを復元したことを示します。</span><span class="sxs-lookup"><span data-stu-id="9133d-103">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="9133d-104">**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9133d-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9133d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9133d-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="9133d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9133d-106">Properties</span></span>

<span data-ttu-id="9133d-107">なし。</span><span class="sxs-lookup"><span data-stu-id="9133d-107">None.</span></span> <span data-ttu-id="9133d-108">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="9133d-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="9133d-109">備考</span><span class="sxs-lookup"><span data-stu-id="9133d-109">Remarks</span></span>

<span data-ttu-id="9133d-110">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="9133d-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/restoreaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
