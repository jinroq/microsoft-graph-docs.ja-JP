# <a name="worksheetprotection-resource-type"></a>WorksheetProtection リソースの種類

シート オブジェクトの保護を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[WorksheetProtection を取得する](../api/worksheetprotection_get.md) | [WorksheetProtection](worksheetprotection.md) |worksheetProtection オブジェクトのプロパティと関係を読み取ります。|
|[Protect](../api/worksheetprotection_protect.md)|なし|ワークシートを保護します。ワークシートが保護されている場合はスローします。|
|[Unprotect](../api/worksheetprotection_unprotect.md)|なし|ワークシートの保護を解除します。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|protected|boolean|ワークシートが保護されているかどうかを示します。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|options|[WorksheetProtectionOptions](worksheetprotectionoptions.md)|シートの保護のオプション。読み取り専用。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->