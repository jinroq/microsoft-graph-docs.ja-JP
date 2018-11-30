---
title: plannerGroup リソースの種類
description: '**PlannerGroup**リソースでは、グループの計画のリソースへのアクセスを提供します。 使用可能なプロパティが含まれていません。'
ms.openlocfilehash: 3a2bb9cfd90a36f6b0a2148e0d789ac97b2199fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022655"
---
# <a name="plannergroup-resource-type"></a>plannerGroup リソースの種類

**plannerGroup** リソースは、[group](group.md) の Planner リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[plans を一覧表示する](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md) コレクション| **plannerPlan** オブジェクト コレクションを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。**plannerGroup** の識別子|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|plans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。Null 許容型。グループが所有する [plannerPlans](plannerplan.md) を返します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->