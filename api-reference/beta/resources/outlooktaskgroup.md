---
title: outlookTaskGroup リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダー (outlookTaskFolder) のグループです。 '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5e885c4c8cc2abe4b3890635e010d495267dc877
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878772"
---
# <a name="outlooktaskgroup-resource-type"></a>outlookTaskGroup リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Outlook のタスク ( [outlookTask](outlooktask.md)オブジェクトのコレクション) を含むフォルダー ([outlookTaskFolder](outlooktaskfolder.md)) のグループです。 

Outlook には、名前を変更または削除することができない既定のタスク グループ `My Tasks` があります。 ただし、タスク グループを作成することはできます。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[OutlookTaskGroup を取得します。](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |プロパティと指定した Outlook のタスク グループの関係を取得します。|
|[OutlookTaskFolder を作成します。](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Outlook の仕事フォルダーを作成します。|
|[リスト taskFolders](../api/outlooktaskgroup-list-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)コレクション| Outlook の仕事フォルダーのコレクションを取得します。|
|[Update](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |Outlook のタスク グループの書き込み可能なプロパティを更新します。 |
|[Delete](../api/outlooktaskgroup-delete.md) | なし |指定された Outlook タスク グループを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|changeKey|String|タスク グループのバージョン。|
|groupKey|Edm.Guid|タスク グループの一意の GUID 識別子。|
|id|String|タスク グループの一意の文字列識別子です。 読み取り専用です。|
|isDefaultGroup|ブール型|タスク グループが既定のタスク グループの場合は true。|
|名前|String|タスク グループの名前。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|taskFolders|[outlookTaskFolder](outlooktaskfolder.md)コレクション| タスク グループ内のタスク フォルダーのコレクションです。 読み取り専用です。 Null 許容型。|

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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
