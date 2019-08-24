---
title: 添付ファイル リソースの種類
description: 関連コンテンツをイベントに追加できます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: da7e66d1edbda224fe547b7e7afc8fd88dc5e5aa
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622637"
---
# <a name="attachment-resource-type"></a>添付ファイル リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添付ファイルの形式で、関連するコンテンツをユーザー[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook タスク](../resources/outlooktask.md)、またはグループ[投稿](../resources/post.md)に追加できます。

**attachment** は、次の派生型の添付ファイルの基本リソースです。

* ファイル ([fileAttachment](../resources/fileattachment.md) リソース)
* 項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)
* ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)

グループの予定表のイベントは、添付ファイルをサポートしていません。

## <a name="methods"></a>メソッド

次のメソッドは、派生型の添付ファイル (**fileAttachment**、**itemAttachment**、または **referenceAttachment**) のすべてに適用されます。

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[添付ファイルを取得する](../api/attachment-get.md) | [attachment](attachment.md) |ユーザーイベント、メッセージ、Outlook タスク、または投稿に添付されている添付ファイルのプロパティと関係を読み取ります。|
|[ユーザーイベントに添付ファイルを追加する](../api/event-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルをユーザーの予定表のイベントに追加します。|
|[メッセージに添付ファイルを追加する](../api/message-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルをメッセージに追加します。|
|[Outlook タスクに添付ファイルを追加する](../api/outlooktask-post-attachments.md) | [attachment](attachment.md) |Outlook タスクにファイル、アイテム、またはリンクの添付ファイルを追加します。|
|[投稿に添付ファイルを追加する](../api/post-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルを投稿に追加します。|
|[ユーザーイベントの添付ファイルを一覧表示する](../api/event-list-attachments.md) | [attachment](attachment.md) コレクション | ユーザーの予定表にあるイベントの添付ファイルの一覧を取得します。 |
|[メッセージの添付ファイルを一覧表示する](../api/message-list-attachments.md) | [attachment](attachment.md) コレクション | メッセージの添付ファイルの一覧を取得します。 |
|[Outlook タスクの添付ファイルを一覧表示する](../api/outlooktask-list-attachments.md) | [attachment](attachment.md) コレクション | Outlook タスクの添付ファイルの一覧を取得します。 |
|[投稿の添付ファイルを一覧表示する](../api/post-list-attachments.md) | [attachment](attachment.md) コレクション | 投稿の添付ファイルの一覧を取得します。 |
|[削除](../api/attachment-delete.md) | None |イベント、メッセージ、Outlook タスク、または投稿の添付ファイルを削除します。 |

## <a name="properties"></a>プロパティ

次に、添付ファイル リソースの基本プロパティを示します。他のプロパティについては、特定の種類の添付ファイル ([fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md)、または [referenceAttachment](../resources/referenceattachment.md)) を参照してください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contentType|String|MIME タイプ。|
|id|文字列| 読み取り専用。|
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
  "suppressions": []
}
-->
