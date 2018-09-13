# <a name="filesecuritystate-resource-type"></a>fileSecurityState リソースの種類

アラートに関連するファイル (プロセスではない) に関する情報が含まれています。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。|
|名前|文字列|ファイル名（パスなし）。|
|パス|文字列|ファイル/ imageFileのフルファイルパス。|
|riskScore|文字列|プロバイダー生成された計算されるリスクの警告ファイルのスコアです。 1 パーセンテージ相当する 0 - 1 の値の範囲を推奨します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->