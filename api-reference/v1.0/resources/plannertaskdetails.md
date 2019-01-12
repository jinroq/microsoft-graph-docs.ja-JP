---
title: plannerTaskDetails リソースの種類
description: '**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 task オブジェクトには詳細オブジェクトがあります。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75e17200dc52fff385c7be8fb0269a3da20464b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956011"
---
# <a name="plannertaskdetails-resource-type"></a>plannerTaskDetails リソースの種類

**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 [task](plannertask.md) オブジェクトには詳細オブジェクトがあります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |**plannerTaskDetails** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |**plannerTaskDetails** オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|タスク上のチェックリスト項目のコレクション。|
|説明|String|タスクの説明|
|id|String| 読み取り専用です。 タスクの詳細の ID です。 28 の文字、大文字小文字を区別することをお勧めします。 サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。|
|previewType|string|タスクに表示されるプレビューの種類を設定します。 可能な値: `automatic`、 `noPreview`、 `checklist`、 `description`、 `reference`。 設定すると`automatic`、タスクを表示するアプリケーションで表示されているプレビューを選択します。|
|references|[plannerExternalReferences](plannerexternalreferences.md)|タスク上の参照のコレクションです。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
