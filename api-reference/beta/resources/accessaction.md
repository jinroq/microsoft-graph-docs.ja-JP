---
author: daspek
ms.author: dspektor
ms.date: 09/12/2018
title: AccessAction
localization_priority: Normal
ms.openlocfilehash: bef6444fd42080c6f5b7cdabb69dbe9a50bab8d6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511521"
---
# <a name="accessaction-resource-type"></a><span data-ttu-id="73de3-102">accessAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73de3-102">accessAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73de3-103">[**ItemActivity**]の**accessAction**リソースが存在すること[activity]活動がアイテムをアクセスすることを示します。</span><span class="sxs-lookup"><span data-stu-id="73de3-103">The presence of the **accessAction** resource on an [**itemActivity**][activity] indicates that the activity accessed an item.</span></span>

><span data-ttu-id="73de3-104">**注:** 活動レコードのアクセスは現在 SharePoint とビジネスの OneDrive にします。</span><span class="sxs-lookup"><span data-stu-id="73de3-104">**Note:** Access activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="73de3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73de3-105">Properties</span></span>

<span data-ttu-id="73de3-106">この種類のリソースには、プロパティはありません。</span><span class="sxs-lookup"><span data-stu-id="73de3-106">This resource type has no properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73de3-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73de3-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.accessAction"
}-->

```json
{
}
```


<!--
{
  "type": "#page.annotation",
  "description": "The AccessAction object provides information about accesses of an item.",
  "keywords": "activities,activity,action,access",
  "section": "documentation",
  "tocPath": "Resources/AccessAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
