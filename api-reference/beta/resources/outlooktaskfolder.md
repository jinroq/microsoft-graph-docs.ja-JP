---
title: outlookTaskFolder リソースの種類
description: 'Outlook のタスク (outlookTask オブジェクトのコレクション) を含むフォルダーです。 '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4b4c4bade46022b30c6e4e1f50aae58d32656f0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882930"
---
# <a name="outlooktaskfolder-resource-type"></a>outlookTaskFolder リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Outlook のタスク ( [outlookTask](outlooktask.md)オブジェクトのコレクション) を含むフォルダーです。 

Outlook では、既定のタスク グループ `My Tasks` には、ユーザーのメールボックス用の既定のタスク フォルダー `Tasks` が含まれています。 これらの既定のタスク グループとフォルダーの名前を変更したり削除したりすることはできませんが、タスク グループとタスク フォルダーを作成することはできます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[OutlookTaskFolder を取得します。](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |プロパティと指定した Outlook の仕事フォルダーの関係を取得します。|
|[OutlookTask を作成します。](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| 指定されたタスクのフォルダーに Outlook のタスクを作成します。|
|[List tasks](../api/outlooktaskfolder-list-tasks.md) |[outlookTask](outlooktask.md)コレクション| 指定したフォルダーに Outlook のすべてのタスクを取得します。|
|[Update](../api/outlooktaskfolder-update.md) | [outlookTaskFolder](outlooktaskfolder.md)   |Outlook の仕事フォルダーの書き込み可能なプロパティを更新します。 |
|[Delete](../api/outlooktaskfolder-delete.md) | なし |指定した Outlook の仕事フォルダーを削除します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |新規または既存の Outlook タスク フォルダー内の 1 つまたは複数の単一値の拡張プロパティを作成します。   |
|[拡張プロパティを単一値を持つタスク フォルダーを取得します。](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | 拡張プロパティを使用して単一の値が含まれている Outlook の仕事フォルダーを取得する`$expand`または`$filter`。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | 新規または既存の Outlook タスク フォルダー内の 1 つまたは複数の値を複数の拡張プロパティを作成します。  |
|[拡張プロパティ値を複数の作業フォルダーを取得します。](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | 使用して複数の値の拡張プロパティを含む Outlook の仕事フォルダーを取得する`$expand`。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|changeKey|String|タスク フォルダーのバージョン。|
|id|String|タスク フォルダーでは、ユーザーのメールボックス内で一意の識別子です。 読み取り専用です。|
|isDefaultFolder|ブール型|フォルダーが既定のタスク フォルダーである場合は true。|
|名前|String|タスク フォルダーの名前。|
|parentGroupKey|Guid|タスク フォルダーの親グループの一意の GUID 識別子。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection|複数値のコレクションでは、仕事フォルダーに対して定義されたプロパティを拡張できます。 読み取り専用です。 Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection|仕事フォルダーに対して定義されている拡張プロパティを単一値のコレクションです。 読み取り専用です。 Null 許容型。|
|tasks|[outlookTask](outlooktask.md)コレクション|対象タスク フォルダー内のタスク。 読み取り専用です。 Null 許容型。|

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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
