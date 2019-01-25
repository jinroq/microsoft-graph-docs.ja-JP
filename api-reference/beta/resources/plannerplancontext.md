---
title: plannerPlanContext リソースの種類
description: '**PlannerPlanContext**リソースでは、プランナーの外部のユーザー エクスペリエンスの plannerPlan との関係を表します。 プランナーでプランは、その経験のコンテキストで作業を追跡するために、マイクロソフトのチームなど、他の経験で提示されることができます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509239"
---
# <a name="plannerplancontext-resource-type"></a>plannerPlanContext リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerPlanContext**リソースでは、計画外のユーザー エクスペリエンスには、 [plannerPlan](plannerplan.md)との関係を表します。 プランナーでプランは、その経験のコンテキストで作業を追跡するために、マイクロソフトのチームなど、他の経験で提示されることができます。
**PlannerPlanContext**エントリの reresents の経験は、 **ownerAppId**プロパティに基づいて識別できます。
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: コンテキストのエントリは、マイクロソフトのチームに属しています。
 - 00000003-0000-0ff1-ce00-000000000000: コンテキスト項目が SharePoint に所属します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|associationType|String|Null 許容型。 [PlannerPlan](plannerplan.md)とアプリケーション間の関連のアプリケーションで定義されている型。 アプリケーションは、同じ[plannerPlan](plannerplan.md)を別の種類の関係を追跡するためにこの情報を使用できます。|
|createdDateTime|DateTimeOffset|読み取り専用です。 日付と時刻**plannerPlanContext**が作成されました。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|displayNameSegments|String コレクション|外部環境の名前のセグメントです。 セグメントでは、リレーションシップを表示するには、他のアプリケーションを可能にする階層構造を表します。|
|ownerAppId|String|読み取り専用です。 **PlannerPlanContext**を作成するアプリケーションの ID です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
