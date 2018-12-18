---
title: outlookTask リソースの種類
description: '作業項目を追跡することができる Outlook のアイテム。 '
author: angelgolfer-ms
ms.openlocfilehash: 959e7ee7d6b1844d4b66b8ab53747e26aa91d492
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335232"
---
# <a name="outlooktask-resource-type"></a>outlookTask リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

作業項目を追跡することができる Outlook のアイテム。 

定期的なアイテムは、通知を必要とするかどうか、期日と実際の終了日と時間、進行状況や状態、開始日を追跡するためにタスクを使用することができます。

**OutlookTask**リソース内の日付に関連するプロパティを以下に示します。

- CompletedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

既定では、POST、GET、パッチ、および[完全な](../api/outlooktask-complete.md)操作は、UTC で、残りの応答に日付に関連するプロパティを返します。 ヘッダーを使用して、応答内のすべての日付関連プロパティを UTC 以外のタイム ゾーンで表すことができます。`Prefer: outlook.timezone` 次の例では、対応する応答の日付関連プロパティが EST で返されています。

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[OutlookTask を取得します。](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |ユーザーのメールボックスのプロパティと、Outlook のタスクの関係を取得します。|
|[Update](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |Outlook の仕事の書き込み可能なプロパティを変更します。 |
|[Delete](../api/outlooktask-delete.md) | なし |ユーザーのメールボックス内の指定されたタスクを削除します。 |
|[Complete](../api/outlooktask-complete.md)|[outlookTask](outlooktask.md)コレクション|**CompletedDateTime**プロパティに現在の日付、および**状態**のプロパティを設定する Outlook のタスクを完了`completed`。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/outlooktask-list-attachments.md) |[attachment](attachment.md) コレクション| Outlook の仕事のすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/outlooktask-post-attachments.md) |[attachment](attachment.md)| タスクに添付ファイルとして、ファイル、アイテム (メッセージ、イベント、または取引先担当者)、またはリンクをファイルに追加します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |新規または既存の Outlook タスクの 1 つまたは複数の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを使用してタスクを取得します。](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | 拡張プロパティを使用して単一の値が含まれている Outlook のタスクを取得する`$expand`または`$filter`。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | 新規または既存の Outlook タスクの 1 つまたは複数の値を複数の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを使用してタスクを取得します。](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | 使用して複数の値の拡張プロパティを含む Outlook のタスクを取得する`$expand`。 |

## <a name="properties"></a>Properties
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|担当者|String|タスクが割り当てられているユーザーの名前。|
|body|[itemBody](itembody.md)|通常はタスクに関する情報を含むタスク本体。HTML 型のみがサポートされていることに注意してください。|
|categories|String コレクション|タスクに関連付けられたカテゴリ。 各カテゴリは、ユーザーが定義されている[outlookCategory](outlookcategory.md)の**表示名**のプロパティに対応します。|
|changeKey|String|タスクのバージョン。|
|CompletedDateTime|[dateTimeTimeZone](datetimetimezone.md)|タスクが終了した日付 (指定のタイム ゾーン)。|
|createdDateTime|DateTimeOffset|日付と時刻、タスクが作成された日時です。 既定では、UTC であります。 要求ヘッダーにカスタム タイム ゾーンを使用できます。 プロパティの値は、ISO 8601 形式を使用します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|タスクが終了する予定の日時 (指定のタイム ゾーン)。|
|hasAttachments|ブール型|タスクに添付ファイルが含まれている場合、true に設定します。|
|id|String|タスクの一意識別子。 読み取り専用。|
|importance|string|イベントの重要度。 可能な値は `low`、`normal`、`high` です。|
|isReminderOn|Boolean|ユーザーにタスクを通知するアラートを設定する場合は、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|日付と、タスクが最後に修正されました。 既定では、UTC であります。 要求ヘッダーにカスタム タイム ゾーンを使用できます。 プロパティの値は、ISO 8601 形式を使用し、UTC 時刻が常に。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|owner|String|タスクを作成したユーザーの名前。|
|parentFolderId|String|タスクの親フォルダーの一意の識別子。|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|タスクの繰り返しパターン。|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|タスクのアラーム通知を行う日時。|
|sensitivity|string|タスクのプライバシーのレベルを示します。 可能な値は、`normal`、`personal`、`private`、`confidential` です。|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|タスクを開始する日付 (指定のタイム ゾーン)。|
|status|string|状態またはタスクの進行状況を示します。 可能な値は、`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred` です。|
|subject|String|タスクのタイトルまたは簡単な説明。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) コレクション|タスクの[fileAttachment](fileattachment.md)、 [itemAttachment](itemattachment.md)、および[referenceAttachment](referenceattachment.md)の添付ファイルのコレクションです。  読み取り専用です。 Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection|複数値のコレクションは、タスクに対して定義されたプロパティを拡張します。 読み取り専用です。 Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection|単一値のコレクションでは、タスクに対して定義されたプロパティを拡張します。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->