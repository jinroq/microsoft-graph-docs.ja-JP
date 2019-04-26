---
title: referenceAttachment リソースの種類
description: 'OneDrive for business のクラウドドライブ上のフォルダーまたはファイル (テキストファイルや Word 文書など) またはその他のサポートされているストレージの場所へのリンクは、 '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563097"
---
# <a name="referenceattachment-resource-type"></a>referenceAttachment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneDrive for business クラウドドライブ上のフォルダーまたはファイル (テキストファイルや Word 文書など) またはその他のサポートされているストレージの場所を、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook のタスク](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付したリンク。

[添付ファイル](attachment.md)から派生します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[取得](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |referenceAttachment オブジェクトのプロパティと関係を読み取ります。|
|[削除](../api/attachment-delete.md) | なし |referenceAttachment オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contentType|String|添付ファイルのコンテンツ タイプ。 省略可能。|
|id|String|添付ファイル ID。読み取り専用です。|
|isFolder|ブール型|添付ファイルがフォルダーへのリンクであるかどうかを指定します。 **sourceurl**がフォルダーへのリンクの場合は、true に設定する必要があります。 省略可能。|
|isInline|ブール値|添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。 省略可能。|
|lastModifiedDateTime|DateTimeOffset|添付ファイルが最後に変更された日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 省略可能。|
|name|String|埋め込まれた添付ファイルを表すアイコンの下に表示されるテキスト。 実際のファイル名である必要はありません。 必須。|
|権|ReferenceAttachmentPermissions|**providertype**のプロバイダーの種類によって添付ファイルに付与されるアクセス許可を指定します。 可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。 省略可能。|
|previewUrl|String|イメージ URL の参照添付ファイルにのみ適用され、プレビューイメージを取得します。 **thumbnailUrl**および**プレビュー url**は、 **sourceurl**が画像ファイルを識別する場合にのみ使用します。 省略可能。|
|providerType|ReferenceAttachmentProviders|この contentType の添付ファイルをサポートするプロバイダーの種類。 可能な値は、`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox` です。 省略可能。|
|size|Int32|参照添付ファイルのメッセージに格納されているメタデータのサイズ (バイト単位)。 この値は実際のファイルのサイズを示すものではありません。 省略可能。|
|sourceUrl|文字列|添付ファイルの内容を取得するための URL。 これがフォルダーへの URL である場合、outlook または web 上の outlook でフォルダーが正しく表示されるようにするには、 **isfolder**を true に設定します。 必須です。|
|thumbnailUrl|String|サムネイルイメージを取得するために、イメージ URL の参照添付ファイルにのみ適用されます。 **thumbnailUrl**および**プレビュー url**は、 **sourceurl**が画像ファイルを識別する場合にのみ使用します。 省略可能。|

## <a name="relationships"></a>関係
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
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
