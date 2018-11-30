---
title: referenceAttachment リソースの種類
description: '接続されているフォルダーや、OneDrive ビジネス クラウド ドライブ、またはその他のサポートされているストレージの場所にテキスト ファイルまたは Word 文書) などのファイルへのリンク '
ms.openlocfilehash: e9885c3a0e5c7f723303d7d6461f4c07dbed6bf6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072252"
---
# <a name="referenceattachment-resource-type"></a>referenceAttachment リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
|isFolder|ブール値|添付ファイルがフォルダーへのリンクであるかどうかを指定します。 True を設定**し直すこと**は、フォルダーへのリンクを設定する必要があります。 省略可能。|
|isInline|ブール値|添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。 省略可能。|
|lastModifiedDateTime|DateTimeOffset|添付ファイルが最後に変更された日時です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 省略可能。|
|名前|String|埋め込まれた添付ファイルを表すアイコンの下に表示されるテキストです。 これは、実際のファイル名を指定するのには必要ありません。 必須。|
|アクセス許可|ReferenceAttachmentPermissions|**プロバイダーの種類**のプロバイダーの種類によって、添付ファイルに付与するアクセス許可を指定します。 可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。 省略可能。|
|previewUrl|String|イメージのプレビュー イメージを取得する URL の参照添付ファイルのみに適用されます。 **直すこと**は、イメージ ファイルを指定するときにのみ、 **thumbnailUrl**および**previewUrl**を使用します。 省略可能。|
|プロバイダーの種類|ReferenceAttachmentProviders|このコンテンツ タイプの添付ファイルをサポートするプロバイダーの型。 可能な値は、`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox` です。 省略可能。|
|size|Int32|バイト内の参照の添付ファイルをメッセージに格納されているメタデータのサイズです。 この値は実際のファイルのサイズを示すものではありません。 省略可能。|
|sourceUrl|String|添付ファイルのコンテンツを取得する URL です。 フォルダーへの URL の場合は、し、Outlook または Outlook web 上で正しく表示されるフォルダーの**isFolder** true に設定します。 必須。|
|thumbnailUrl|String|イメージのサムネイル イメージを取得する URL の参照添付ファイルのみに適用されます。 **直すこと**は、イメージ ファイルを指定するときにのみ、 **thumbnailUrl**および**previewUrl**を使用します。 省略可能。|

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
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
