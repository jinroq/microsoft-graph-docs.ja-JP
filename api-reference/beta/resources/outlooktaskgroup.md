---
title: outlooktaskgroup リソースの種類
description: 'Outlook のタスク (outlooktask オブジェクトのコレクション) を含むフォルダーのグループ (outlooktaskfolder)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 486261d80b8faad7a5969f8f1ce198479e39583c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568602"
---
# <a name="outlooktaskgroup-resource-type"></a>outlooktaskgroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Outlook のタスク ( [outlooktask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーのグループ ([outlooktaskfolder](outlooktaskfolder.md))。 

Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。 ただし、タスク グループを作成することはできます。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[outlooktaskgroup の取得](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |指定された Outlook タスクグループのプロパティとリレーションシップを取得します。|
|[outlooktaskfolder の作成](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Outlook のタスクフォルダーを作成します。|
|[taskfolders を一覧表示する](../api/outlooktaskgroup-list-taskfolders.md) |[outlooktaskfolder](outlooktaskfolder.md)コレクション| Outlook タスクフォルダーのコレクションを取得します。|
|[更新する](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |Outlook タスクグループの書き込み可能なプロパティを更新します。 |
|[削除](../api/outlooktaskgroup-delete.md) | なし |指定された Outlook タスクグループを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|changeKey|String|タスク グループのバージョン。|
|groupkey|Edm.Guid|タスク グループの一意の GUID 識別子。|
|id|文字列型 (String)|タスクグループの一意の文字列識別子。 読み取り専用。|
|isdefaultgroup|ブール型|タスク グループが既定のタスク グループの場合は true。|
|name|String|タスク グループの名前。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|taskfolders|[outlooktaskfolder](outlooktaskfolder.md)コレクション| タスクグループ内のタスクフォルダーのコレクション。 読み取り専用。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
