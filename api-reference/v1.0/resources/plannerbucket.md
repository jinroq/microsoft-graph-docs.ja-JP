---
title: plannerBucket リソースの種類
description: ) Office 365 のプランでの作業をします。 PlannerPlan に含まれ、plannerTasks のコレクションを持つことができます。
author: TarkanSevilmis
ms.openlocfilehash: 09c9fab569a819f0545e5c851da12be98b45b150
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331445"
---
# <a name="plannerbucket-resource-type"></a>plannerBucket リソースの種類

**PlannerBucket** リソースは、Office 365 の計画におけるタスクのバケット (または "カスタム列") を表します。これは [plannerPlan](plannerplan.md) に含まれており、[plannerTasks](plannertask.md) のコレクションを持ちます。



## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |**plannerBucket** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[List plannerTasks](../api/plannerbucket-list-tasks.md) |[plannerTask](plannertask.md) コレクション| **plannerTask** オブジェクト コレクションを取得します。|
|[Create](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | 新しい **plannerBucket** オブジェクトを作成します。 |
|[Update](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |**plannerBucket** オブジェクトを更新します。 |
|[Delete](../api/plannerbucket-delete.md) | なし |**plannerBucket** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|String| 読み取り専用です。 バケットの ID です。 28 の文字、大文字小文字を区別することをお勧めします。 サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。|
|名前|String|バケットの名前。|
|orderHint|String|リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|
|planId|String|バケットが所属する計画の ID。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。Null 許容型。バケットに含まれるタスクのコレクション。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->