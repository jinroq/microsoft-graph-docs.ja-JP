---
title: plannerPlanContext リソースの種類
description: '**PlannerPlanContext**リソースでは、プランナーの外部のユーザー エクスペリエンスの plannerPlan との関係を表します。 プランナーでプランは、その経験のコンテキストで作業を追跡するために、マイクロソフトのチームなど、他の経験で提示されることができます。'
ms.openlocfilehash: 84512c03081a3e1fd2b15456c64cecf3f9c39435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070633"
---
# <a name="plannerplancontext-resource-type"></a>plannerPlanContext リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**PlannerPlanContext**リソースでは、計画外のユーザー エクスペリエンスには、 [plannerPlan](plannerplan.md)との関係を表します。 プランナーでプランは、その経験のコンテキストで作業を追跡するために、マイクロソフトのチームなど、他の経験で提示されることができます。
**PlannerPlanContext**エントリの reresents の経験は、 **ownerAppId**プロパティに基づいて識別できます。
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: コンテキストのエントリは、マイクロソフトのチームに属しています。
 - 00000003-0000-0ff1-ce00-000000000000: コンテキスト項目が SharePoint に所属します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|associationType|String|Null 許容型。 [PlannerPlan](plannerplan.md)とアプリケーション間の関連のアプリケーションで定義されている型。 アプリケーションは、同じ[plannerPlan](plannerplan.md)を別の種類の関係を追跡するためにこの情報を使用できます。|
|createdDateTime|DateTimeOffset|読み取り専用。 日付と時刻**plannerPlanContext**が作成されました。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|displayNameSegments|String コレクション|外部環境の名前のセグメントです。 セグメントでは、リレーションシップを表示するには、他のアプリケーションを可能にする階層構造を表します。|
|ownerAppId|String|読み取り専用。 **PlannerPlanContext**を作成するアプリケーションの ID です。|

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
