---
title: outlooktaskfolder リソースの種類
description: 'Outlook のタスク (outlooktask オブジェクトのコレクション) が格納されているフォルダー。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eb61936b9ede67d35127db07c92ba8b7517fe623
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568605"
---
# <a name="outlooktaskfolder-resource-type"></a>outlooktaskfolder リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Outlook のタスク ( [outlooktask](outlooktask.md)オブジェクトのコレクション) が格納されているフォルダー。 

Outlook では、既定のタスク グループ `My Tasks` には、ユーザーのメールボックス用の既定のタスク フォルダー `Tasks` が含まれています。 これらの既定のタスク グループとフォルダーの名前を変更したり削除したりすることはできませんが、タスク グループとタスク フォルダーを作成することはできます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[outlooktaskfolder の取得](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |指定された Outlook タスクフォルダーのプロパティとリレーションシップを取得します。|
|[outlooktask の作成](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| 指定したタスクフォルダーに Outlook のタスクを作成します。|
|[タスクを一覧表示する](../api/outlooktaskfolder-list-tasks.md) |[outlookTask](outlooktask.md) コレクション| 指定したフォルダー内のすべての Outlook タスクを取得します。|
|[更新する](../api/outlooktaskfolder-update.md) | [outlookTaskFolder](outlooktaskfolder.md)   |Outlook タスクフォルダーの書き込み可能なプロパティを更新します。 |
|[削除](../api/outlooktaskfolder-delete.md) | なし |指定された Outlook タスクフォルダーを削除します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |新規または既存の Outlook タスクフォルダーに、1つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つタスクフォルダーを取得する](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | または`$expand` `$filter`を使用して、単一値の拡張プロパティを含む Outlook タスクフォルダーを取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | 新規または既存の Outlook タスクフォルダーに、1つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つタスクフォルダーを取得する](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | を使用`$expand`して、複数値の拡張プロパティを含む Outlook のタスクフォルダーを取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|changeKey|String|タスク フォルダーのバージョン。|
|id|文字列型 (String)|ユーザーのメールボックス内で一意のタスクフォルダーの識別子。 読み取り専用。|
|isdefaultfolder|Boolean|フォルダーが既定のタスク フォルダーである場合は true。|
|name|String|タスク フォルダーの名前。|
|parentgroupkey|Guid|タスク フォルダーの親グループの一意の GUID 識別子。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection|タスクフォルダーに対して定義されている複数値の拡張プロパティのコレクション。 読み取り専用。 Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection|タスクフォルダーに対して定義されている単一値の拡張プロパティのコレクションです。 読み取り専用。 Null 許容型。|
|tasks|[outlookTask](outlooktask.md) コレクション|対象タスク フォルダー内のタスク。 読み取り専用。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
