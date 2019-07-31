---
title: outlookTaskGroup リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダーのグループ (outlookTaskFolder)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d519e18723ac9fbd38e7cec64a6758b0c9396bc2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966280"
---
# <a name="outlooktaskgroup-resource-type"></a>outlookTaskGroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Outlook のタスク ( [Outlooktask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーのグループ ([outlooktaskfolder](outlooktaskfolder.md))。 

Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。 ただし、タスク グループを作成することはできます。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[OutlookTaskGroup の取得](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |指定された Outlook タスクグループのプロパティとリレーションシップを取得します。|
|[OutlookTaskFolder の作成](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Outlook のタスクフォルダーを作成します。|
|[TaskFolders を一覧表示する](../api/outlooktaskgroup-list-taskfolders.md) |[Outlooktaskfolder](outlooktaskfolder.md)コレクション| Outlook タスクフォルダーのコレクションを取得します。|
|[Update](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |Outlook タスクグループの書き込み可能なプロパティを更新します。 |
|[Delete](../api/outlooktaskgroup-delete.md) | None |指定された Outlook タスクグループを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|changeKey|String|タスク グループのバージョン。|
|groupKey|Edm.Guid|タスク グループの一意の GUID 識別子。|
|id|文字列|タスクグループの一意の文字列識別子。 読み取り専用です。|
|isDefaultGroup|ブール型|タスク グループが既定のタスク グループの場合は true。|
|name|String|タスク グループの名前。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|taskFolders|[Outlooktaskfolder](outlooktaskfolder.md)コレクション| タスクグループ内のタスクフォルダーのコレクション。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
