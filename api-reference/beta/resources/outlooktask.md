---
title: outlookTask リソースの種類
description: '作業アイテムを追跡することができる Outlook アイテム。 '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 231cb227c33e9f58e0dbe87dbf832b86bf2f017f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459602"
---
# <a name="outlooktask-resource-type"></a>outlookTask リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作業アイテムを追跡することができる Outlook アイテム。

タスクを使用すると、開始日時、期限日時、実際の完了日時、進行状況や状態、定期的かどうか、通知が必要かどうかを追跡できます。

**outlookTask** リソースの日付関連プロパティには次が含まれます。

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

既定では、POST、GET、PATCH、および [complete](../api/outlooktask-complete.md) 操作は、REST 応答の日付関連プロパティを UTC で返します。
`Prefer: outlook.timezone` ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。 次の例では、対応する応答の日付関連プロパティが EST で返されています。

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[outlookTask を取得する](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |ユーザーのメールボックスにある Outlook タスクのプロパティとリレーションシップを取得します。|
|[更新する](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |Outlook タスクの書き込み可能なプロパティを変更します。 |
|[削除する](../api/outlooktask-delete.md) | なし |ユーザーのメールボックス内の指定されたタスクを削除します。 |
|[完了する](../api/outlooktask-complete.md)|[outlookTask](outlooktask.md) コレクション|**completedDateTime** プロパティを現在の日付に設定し、**status** プロパティを `completed` に設定する Outlook タスクを完了します。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/outlooktask-list-attachments.md) |[attachment](attachment.md) コレクション| Outlook タスクのすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/outlooktask-post-attachments.md) |[attachment](attachment.md)| タスクへの添付としてファイル、アイテム (メッセージ、イベント、連絡先)、またはファイルへのリンクを追加します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |新規または既存の Outlook タスクに、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つタスクを取得する](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む Outlook タスクを取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | 新規または既存の Outlook タスクに、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つタスクの取得](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | `$expand` を使用して、複数値の拡張プロパティを含む Outlook タスクを取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedTo|String|Outlook でタスクが割り当てられているユーザーの名前。 読み取り専用です。|
|body|[itemBody](itembody.md)|通常はタスクに関する情報を含むタスク本体。HTML 型のみがサポートされていることに注意してください。|
|categories|String コレクション|タスクに関連付けられたカテゴリ。 各カテゴリは、ユーザーが定義した [outlookCategory](outlookcategory.md) の **displayName** プロパティに対応しています。|
|changeKey|String|タスクのバージョン。|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|タスクが終了した日付 (指定のタイム ゾーン)。|
|createdDateTime|DateTimeOffset|タスクが作成された日時。 既定では、UTC 時間です。 要求ヘッダーでカスタム タイム ゾーンを使用できます。 プロパティの値は、ISO 8601 形式を使用します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|タスクが終了する予定の日時 (指定のタイム ゾーン)。|
|hasAttachments|Boolean|タスクに添付ファイルが含まれている場合、true に設定します。|
|id|String| タスクの一意識別子。 [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] 読み取り専用です。 |
|importance|string|イベントの重要度。 可能な値は、`low`、`normal`、`high` です。|
|isReminderOn|Boolean|ユーザーにタスクを通知するアラートを設定する場合は、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|タスクが最後に変更された日時。 既定では、UTC 時間です。 要求ヘッダーでカスタム タイム ゾーンを使用できます。 プロパティの値は、ISO 8601 形式を使って表され、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|owner|String|タスクを作成したユーザーの名前。|
|parentFolderId|String|タスクの親フォルダーの一意の識別子。|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|タスクの繰り返しパターン。|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|タスクのアラーム通知を行う日時。|
|sensitivity|string|タスクのプライバシーのレベルを示します。 使用可能な値は、`normal`、`personal`、`private`、`confidential` です。|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|タスクを開始する日付 (指定のタイム ゾーン)。|
|status|string|タスクの状態または進行状況を示します。 可能な値は、`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred` です。|
|subject|String|タスクのタイトルまたは簡単な説明。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) コレクション|タスクの [fileAttachment](fileattachment.md)、[itemAttachment](itemattachment.md)、[referenceAttachment](referenceattachment.md) の各添付ファイルのコレクション。  読み取り専用です。 Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション|そのタスクに対して定義された、複数値拡張プロパティのコレクションです。 読み取り専用です。 Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション|そのタスクに対して定義された、単一値拡張プロパティのコレクションです。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookTask"
}-->

```json
{
  "assignedTo": "String",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["String"],
  "changeKey": "String",
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "sensitivity": "string",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "string",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
