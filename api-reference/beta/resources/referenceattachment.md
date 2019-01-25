---
title: referenceAttachment リソースの種類
description: '接続されているフォルダーや、OneDrive ビジネス クラウド ドライブ、またはその他のサポートされているストレージの場所にテキスト ファイルまたは Word 文書) などのファイルへのリンク '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512711"
---
# <a name="referenceattachment-resource-type"></a>referenceAttachment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

フォルダーまたはビジネス クラウド ドライブ、またはその他の OneDrive のテキスト ファイル、または Word 文書) などのファイルへのリンクには、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[ポスト](../resources/post.md)に接続されているストレージの場所がサポートされています。

[添付ファイル](attachment.md)から派生します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[取得](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |referenceAttachment オブジェクトのプロパティと関係を読み取ります。|
|[Delete](../api/attachment-delete.md) | なし |referenceAttachment オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contentType|String|添付ファイルのコンテンツ タイプ。 省略可能。|
|id|String|添付ファイル ID。読み取り専用です。|
|IsFolder|ブール値|添付ファイルがフォルダーへのリンクであるかどうかを指定します。**SourceUrl** がフォルダーへのリンクの場合、true に設定する必要があります。省略可能。|
|isInline|ブール値|添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。 省略可能。|
|lastModifiedDateTime|DateTimeOffset|添付ファイルが最後に変更された日時です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。 省略可能。|
|name|String|埋め込まれた添付ファイルを表すアイコンの下に表示されるテキストです。 これは、実際のファイル名を指定するのには必要ありません。 必須です。|
|アクセス許可|ReferenceAttachmentPermissions|**ProviderType** のプロバイダーの種類によって、添付ファイルに付与されるアクセス許可を指定します。可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。省略可能。|
|PreviewUrl|String|プレビュー イメージを取得するための、イメージの URL の参照添付ファイルのみに適用されます。**SourceUrl** によってイメージ ファイルが識別される場合にのみ、**ThumbnailUrl** と **PreviewUrl** を使用します。省略可能。|
|ProviderType|ReferenceAttachmentProviders|この `other` の添付ファイルをサポートするプロバイダーの種類。可能な値は、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`、 です。省略可能。|
|size|Int32|バイト内の参照の添付ファイルをメッセージに格納されているメタデータのサイズです。 この値は実際のファイルのサイズを示すものではありません。 省略可能。|
|sourceUrl|String|添付ファイルの内容を取得するための URL。フォルダーへの URL の場合、Outlook または Outlook on the web 上でフォルダーが正しく表示されるには、**IsFolder** を true に設定します。必須。|
|ThumbnailUrl|String|サムネイル イメージを取得するための、イメージの URL の参照添付ファイルのみに適用されます。**SourceUrl** によってイメージ ファイルが識別される場合にのみ、**ThumbnailUrl** と **PreviewUrl** を使用します。省略可能。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
