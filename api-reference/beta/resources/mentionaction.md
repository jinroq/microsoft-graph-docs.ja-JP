---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9101ffed094fd78189b73eab511be88c8bf449de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513012"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="a2244-102">MentionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2244-102">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2244-103">**MentionAction** リソースは、ユーザーについて記載した[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a2244-103">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="a2244-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2244-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="a2244-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2244-106">Properties</span></span>

| <span data-ttu-id="a2244-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a2244-107">Property name</span></span> | <span data-ttu-id="a2244-108">種類</span><span class="sxs-lookup"><span data-stu-id="a2244-108">Type</span></span>                       | <span data-ttu-id="a2244-109">説明</span><span class="sxs-lookup"><span data-stu-id="a2244-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="a2244-110">mentionees</span><span class="sxs-lookup"><span data-stu-id="a2244-110">mentionees</span></span>    | <span data-ttu-id="a2244-111">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="a2244-111">[identitySet][] collection</span></span> | <span data-ttu-id="a2244-112">このアクションに記載されているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="a2244-112">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="a2244-114">備考</span><span class="sxs-lookup"><span data-stu-id="a2244-114">Remarks</span></span>

<span data-ttu-id="a2244-115">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="a2244-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
