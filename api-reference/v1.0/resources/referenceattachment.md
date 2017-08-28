# <a name="referenceattachment-resource-type"></a>referenceAttachment リソースの種類

OneDrive for Business のクラウド ドライブまたは他のサポートされている保存場所にあり、イベント、メッセージ、または投稿にアタッチされているファイル (テキスト ファイルまたは Word 文書など) へのリンク。

[添付ファイル](attachment.md)から派生します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[取得](../api/attachment_get.md) | [referenceAttachment](referenceattachment.md) |referenceAttachment オブジェクトのプロパティと関係を読み取ります。|
|[Delete](../api/attachment_delete.md) | なし |referenceAttachment オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contentType|String|添付ファイルのコンテンツ タイプ。|
|id|String|添付ファイル ID。読み取り専用です。|
|isInline|Boolean|添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|添付ファイルが最後に変更された日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|name|String|埋め込まれた添付ファイルを表すアイコンの下に表示されるテキスト。実際のファイル名である必要はありません。|
|size|Int32|添付ファイルのサイズ (バイト単位)。|

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
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
