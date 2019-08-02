---
title: プラン/タスクの詳細リソースの種類
description: "\" **Plan\" Taskdetails**リソースは、タスクに関する追加情報を表します。 各 task オブジェクトには details オブジェクトがあります。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d22c932989b9c0d21350842babd9b4bbf420124c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035169"
---
# <a name="plannertaskdetails-resource-type"></a>プラン/タスクの詳細リソースの種類

" **Plan" Taskdetails**リソースは、タスクに関する追加情報を表します。 各[task](plannertask.md)オブジェクトには details オブジェクトがあります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |**Plan**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |プランの更新方法の**詳細**オブジェクトを表示します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|タスク上のチェックリスト項目のコレクション。|
|description|String|タスクの説明|
|id|文字列| 読み取り専用です。 タスクの詳細の ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。|
|previewType|string|タスクに表示されるプレビューの種類を設定します。 使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。 表示され`automatic`たプレビューに設定した場合は、タスクを表示するアプリによって選択されます。|
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
