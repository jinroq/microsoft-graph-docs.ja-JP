# <a name="uploadsession-resource-type"></a>UploadSession リソースタイプ

**UploadSession** リソースは、OneDrive、OneDrive for Business、または SharePoint のドキュメント ライブラリに、大容量ファイルをアップロードする方法に関する情報を提供します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "expirationDateTime": "timestamp",
  "nextExpectedRanges": ["string"],
  "uploadUrl": "url"
}

```
## <a name="properties"></a>プロパティ


| プロパティ             | 型              |説明|
|:-------------------|:------------------|:----------|
| expirationDateTime | DateTimeOffset    | アップロード セッションの有効期限が切れる日時の UTC 表示。この有効期限に達する前に、完全なファイルをアップロードする必要があります。 |
| nextExpectedRanges | String collection | サーバーのファイルに足りないバイト範囲のコレクションです。これらの範囲は 0 インデックスが作成されており、「開始-終了」形式のものです (例、「0-26」でファイルの最初の 27 バイトを示す)。 |
| uploadUrl          | String            | ファイルのバイト範囲の PUT 要求を受け付ける URL エンドポイントです。 |

## <a name="additional-resources"></a>その他の技術情報

アップロード セッションを使用してファイルをアップロードする方法の詳細については [アップロード セッションで大きいファイルをアップロードする](../api/item_createUploadSession.md) を参照してください。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "uploadSession resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->