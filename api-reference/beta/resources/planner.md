---
title: planner リソースの種類
description: '**Planner**リソースは、planner オブジェクトモデルのエントリポイントです。 シングルトン**プランナー**リソースを返します。  使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2ef94a7507558279e5295239588e2a8eda512882
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009133"
---
# <a name="planner-resource-type"></a>planner リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Planner**リソースは、planner オブジェクトモデルのエントリポイントです。 シングルトン**プランナー**リソースを返します。  使用可能なプロパティは含まれていません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| バケットコレクションへの投稿により、新しい**プラン**を作成します。|
|[Create plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| プランコレクションへの投稿によって、新しい**プラン**を作成します。|
|[Create plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| タスクコレクションへの投稿によって、新しい**プラン**を作成します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用。 **Planner**リソースの識別子。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) コレクション| 読み取り専用です。 Null 許容型。 指定したバケットのコレクションを返します。|
|plans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。 Null 許容型。 指定したプランのコレクションを返します。|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。 Null 許容型。 指定したタスクのコレクションを返します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
