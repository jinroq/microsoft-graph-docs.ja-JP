---
title: referenceAttachment リソースの種類
description: 'OneDrive for Business のクラウドドライブ上のフォルダーまたはファイル (テキストファイルや Word 文書など) またはその他のサポートされているストレージの場所へのリンクは、 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef3e2dd5292ee018c0b72c29c8bd6c33fed00f11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008713"
---
# <a name="referenceattachment-resource-type"></a>referenceAttachment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneDrive for Business クラウドドライブ上のフォルダーまたはファイル (テキストファイルや Word 文書など) またはその他のサポートされているストレージの場所を、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook のタスク](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付したリンク。

[添付ファイル](attachment.md)から派生します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |referenceAttachment オブジェクトのプロパティと関係を読み取ります。|
|[Delete](../api/attachment-delete.md) | None |referenceAttachment オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contentType|String|添付ファイルのコンテンツ タイプ。 省略可能。|
|id|文字列|添付ファイル ID。読み取り専用です。|
|isFolder|ブール型|添付ファイルがフォルダーへのリンクであるかどうかを指定します。 **Sourceurl**がフォルダーへのリンクの場合は、true に設定する必要があります。 省略可能。|
|isInline|Boolean|添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。 省略可能。|
|lastModifiedDateTime|DateTimeOffset|添付ファイルが最後に変更された日時です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 省略可能。|
|name|String|埋め込まれた添付ファイルを表すアイコンの下に表示されるテキスト。 実際のファイル名である必要はありません。 必須。|
|権|Referenceattachmentpermission が|**Providertype**のプロバイダーの種類によって添付ファイルに付与されるアクセス許可を指定します。 可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。 省略可能。|
|previewUrl|String|イメージ URL の参照添付ファイルにのみ適用され、プレビューイメージを取得します。 **ThumbnailUrl**および**プレビュー Url**は、 **sourceurl**が画像ファイルを識別する場合にのみ使用します。 省略可能。|
|providerType|referenceAttachmentProvider|この contentType の添付ファイルをサポートするプロバイダーの種類。 可能な値は、`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox` です。 省略可能。|
|size|Int32|参照添付ファイルのメッセージに格納されているメタデータのサイズ (バイト単位)。 この値は実際のファイルのサイズを示すものではありません。 省略可能。|
|sourceUrl|文字列|添付ファイルの内容を取得するための URL。 これがフォルダーへの URL である場合、Outlook または web 上の Outlook でフォルダーが正しく表示されるようにするには、 **Isfolder**を true に設定します。 必須です。|
|thumbnailUrl|String|サムネイルイメージを取得するために、イメージ URL の参照添付ファイルにのみ適用されます。 **ThumbnailUrl**および**プレビュー Url**は、 **sourceurl**が画像ファイルを識別する場合にのみ使用します。 省略可能。|

## <a name="relationships"></a>リレーションシップ
なし



## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
