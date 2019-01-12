---
title: planner リソースの種類
description: '**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: cf2877d5f413f3e54e1e0e750da1f22d6f9ffd95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925183"
---
# <a name="planner-resource-type"></a>planner リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| バケット コレクションの投稿によって新しい **plannerBucket** を作成します。|
|[Create plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| 計画コレクションの投稿によって新しい **plannerPlan** を作成します。|
|[Create plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| タスク コレクションの投稿によって新しい **plannerTask** を作成します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|String| 読み取り専用です。**planner** リソースの識別子。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) コレクション| 読み取り専用です。Null 許容型。指定されたバケットのコレクションを返します|
|plans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。Null 許容型。指定された計画のコレクションを返します|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。Null 許容型。指定されたタスクのコレクションを返します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
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
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
