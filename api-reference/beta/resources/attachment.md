---
title: 添付ファイル リソースの種類
description: イベントに関連するコンテンツを追加します。
localization_priority: Normal
ms.openlocfilehash: 59e1074cea9508af45cef0b6e61ea223a3ca851e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643151"
---
# <a name="attachment-resource-type"></a>添付ファイル リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または添付ファイルの形式での[投稿](../resources/post.md)に関連するコンテンツを追加できます。

**attachment** は、次の派生型の添付ファイルの基本リソースです。

* ファイル ([fileAttachment](../resources/fileattachment.md) リソース)
* 項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)
* ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)

## <a name="methods"></a>メソッド

次のメソッドは、派生型の添付ファイル (**fileAttachment**、**itemAttachment**、または **referenceAttachment**) のすべてに適用されます。

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[添付ファイルを取得する](../api/attachment-get.md) | [attachment](attachment.md) |プロパティとイベント、メッセージ、Outlook のタスク、または投稿に添付された添付ファイルの関係を参照してください。|
|[イベントに添付ファイルを追加する](../api/event-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルをイベントに追加します。|
|[メッセージに添付ファイルを追加する](../api/message-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルをメッセージに追加します。|
|[Outlook のタスクに添付ファイルを追加します。](../api/outlooktask-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルを Outlook のタスクを追加します。|
|[投稿に添付ファイルを追加する](../api/post-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルを投稿に追加します。|
|[イベントの添付ファイルを一覧表示する](../api/event-list-attachments.md) | [attachment](attachment.md) コレクション | イベントの添付ファイルの一覧を取得します。 |
|[メッセージの添付ファイルを一覧表示する](../api/message-list-attachments.md) | [attachment](attachment.md) コレクション | メッセージの添付ファイルの一覧を取得します。 |
|[Outlook の仕事リストの添付ファイル](../api/outlooktask-list-attachments.md) | [attachment](attachment.md) コレクション | Outlook のタスクの添付ファイルの一覧を取得します。 |
|[投稿の添付ファイルを一覧表示する](../api/post-list-attachments.md) | [attachment](attachment.md) コレクション | 投稿の添付ファイルの一覧を取得します。 |
|[削除](../api/attachment-delete.md) | なし |イベント、メッセージ、Outlook のタスク、または投稿の添付ファイルを削除します。 |

## <a name="properties"></a>プロパティ

次に、添付ファイル リソースの基本プロパティを示します。他のプロパティについては、特定の種類の添付ファイル ([fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md)、または [referenceAttachment](../resources/referenceattachment.md)) を参照してください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contentType|String|MIME タイプ。|
|id|String| 読み取り専用。|
|isInline|Boolean|添付ファイルがインライン添付ファイルの場合は `true`、それ以外の場合は `false`。|
|lastModifiedDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|name|String|添付ファイルの表示名。実際のファイル名である必要はありません。|
|size|Int32|添付ファイルの長さ (バイト単位)。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
