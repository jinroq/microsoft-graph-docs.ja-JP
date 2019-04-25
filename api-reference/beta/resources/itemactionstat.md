---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemactionstat
localization_priority: Normal
ms.openlocfilehash: 39209671b63b991a8fb3ccf1c830c8557fce27c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569985"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="8b84c-102">itemactionstat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b84c-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b84c-103">**itemactionstat**リソースは、一定期間にわたるアクションについての集約された詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="8b84c-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b84c-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b84c-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

## <a name="properties"></a><span data-ttu-id="8b84c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b84c-105">Properties</span></span>

| <span data-ttu-id="8b84c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b84c-106">Property</span></span>    | <span data-ttu-id="8b84c-107">型</span><span class="sxs-lookup"><span data-stu-id="8b84c-107">Type</span></span>  | <span data-ttu-id="8b84c-108">説明</span><span class="sxs-lookup"><span data-stu-id="8b84c-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="8b84c-109">actioncount</span><span class="sxs-lookup"><span data-stu-id="8b84c-109">actionCount</span></span> | <span data-ttu-id="8b84c-110">Int32</span><span class="sxs-lookup"><span data-stu-id="8b84c-110">Int32</span></span> | <span data-ttu-id="8b84c-111">アクションが行われた回数。</span><span class="sxs-lookup"><span data-stu-id="8b84c-111">The number of times the action took place.</span></span> <span data-ttu-id="8b84c-112">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8b84c-112">Read-only.</span></span>
| <span data-ttu-id="8b84c-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="8b84c-113">actorCount</span></span>  | <span data-ttu-id="8b84c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="8b84c-114">Int32</span></span> | <span data-ttu-id="8b84c-115">アクションを実行した個別のアクターの数。</span><span class="sxs-lookup"><span data-stu-id="8b84c-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="8b84c-116">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8b84c-116">Read-only.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactionstat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
