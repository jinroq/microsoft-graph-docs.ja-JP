---
title: 添付ファイル リソースの種類
description: イベントに関連するコンテンツを追加します。
ms.openlocfilehash: 418d8d4e60d12fed5a54f994e14e996c65731926
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022203"
---
# <a name="attachment-resource-type"></a>添付ファイル リソースの種類

関連コンテンツを添付ファイルの形式で[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、または[投稿](../resources/post.md)に追加できます。

**attachment** は、次の派生型の添付ファイルの基本リソースです。

* ファイル ([fileAttachment](../resources/fileattachment.md) リソース)
* 項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)
* ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)


## <a name="methods"></a>メソッド

次のメソッドは、派生型の添付ファイル (**fileAttachment**、**itemAttachment**、または **referenceAttachment**) のすべてに適用されます。

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[添付ファイルを取得する](../api/attachment-get.md) | [attachment](attachment.md) |イベント、メッセージ、または投稿に添付されている添付ファイルのプロパティとリレーションシップを読み取ります。|
|[イベントに添付ファイルを追加する](../api/event-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルをイベントに追加します。|
|[メッセージに添付ファイルを追加する](../api/message-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルをメッセージに追加します。|
|[投稿に添付ファイルを追加する](../api/post-post-attachments.md) | [attachment](attachment.md) |ファイル、アイテム、またはリンクの添付ファイルを投稿に追加します。|
|[イベントの添付ファイルを一覧表示する](../api/event-list-attachments.md) | [attachment](attachment.md) コレクション | イベントの添付ファイルの一覧を取得します。 |
|[メッセージの添付ファイルを一覧表示する](../api/message-list-attachments.md) | [attachment](attachment.md) コレクション | メッセージの添付ファイルの一覧を取得します。 |
|[投稿の添付ファイルを一覧表示する](../api/post-list-attachments.md) | [attachment](attachment.md) コレクション | 投稿の添付ファイルの一覧を取得します。 |
|[削除](../api/attachment-delete.md) | なし |イベント、メッセージ、または投稿の添付ファイルを削除します。 |

## <a name="properties"></a>プロパティ

次に、添付ファイル リソースの基本プロパティを示します。他のプロパティについては、特定の種類の添付ファイル ([fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md)、または [referenceAttachment](../resources/referenceattachment.md)) を参照してください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contentType|String|MIME タイプ。|
|id|String| 読み取り専用。|
|isInline|Boolean|添付ファイルがインライン添付ファイルの場合は `true`、それ以外の場合は `false`。|
|lastModifiedDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|name|String|添付ファイルのファイル名。|
|size|Int32|添付ファイルの長さ (バイト単位)。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
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
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
