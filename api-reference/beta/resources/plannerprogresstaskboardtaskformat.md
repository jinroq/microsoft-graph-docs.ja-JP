---
title: plannerProgressTaskBoardTaskFormat リソースの種類
description: '**plannerProgressTaskBoardTaskFormat** リソースは、タスク ボードの進行状況ビューにタスクを正しく表示するための情報を示します (ビューはタスク オブジェクトの [未開始]、[処理中]、[完了] の列に示す PercentComplete フィールドの状態で整理されます)。各 task にはそれぞれ **plannerProgressTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 58e1b80c61dcb0c58996f65c1fa03c48c4edafbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955927"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>plannerProgressTaskBoardTaskFormat リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**plannerProgressTaskBoardTaskFormat** リソースは、タスク ボードの進行状況ビューにタスクを正しく表示するための情報を示します (ビューはタスク オブジェクトの [未開始]、[処理中]、[完了] の列に示す PercentComplete フィールドの状態で整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerProgressTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/plannerprogresstaskboardtaskformat-update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |**plannerProgressTaskBoardTaskFormat** オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ID|String| 読み取り専用です。 リソースの ID です。 28 の文字、大文字小文字を区別することをお勧めします。 サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。|
|orderHint|String|タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
