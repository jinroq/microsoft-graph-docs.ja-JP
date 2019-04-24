---
title: plannerBucketTaskBoardTaskFormat リソースの種類
description: '**plannerBucketTaskBoardTaskFormat**リソースは、タスクボードのバケットビューでタスクを正しくレンダリングするために使用される情報を表します (割り当てられているバケット内のタスク別に整理されたビュー)。 各タスクには、1つの**plannerBucketTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4982b0b539412058d6d598893b698f12d88bd671
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462243"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>plannerBucketTaskBoardTaskFormat リソースの種類

**plannerBucketTaskBoardTaskFormat**リソースは、タスクボードのバケットビューでタスクを正しくレンダリングするために使用される情報を表します (割り当てられているバケット内のタスク別に整理されたビュー)。 各[タスク](plannertask.md)には、1つの**plannerBucketTaskBoardTaskFormat**オブジェクトが関連付けられています。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |**plannerBucketTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/plannerbuckettaskboardtaskformat-update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)  |**plannerBucketTaskBoardTaskFormat**オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 リソースの ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。|
|orderHint|String|タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
