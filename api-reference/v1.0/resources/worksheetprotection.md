# <a name="worksheetprotection-resource-type"></a>WorksheetProtection リソースの種類

シート オブジェクトの保護を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[WorksheetProtection を取得する](../api/worksheetprotection_get.md) | [WorkbookWorksheetProtection](worksheetprotection.md) |worksheetProtection オブジェクトのプロパティと関係を読み取ります。|
|[保護](../api/worksheetprotection_protect.md)|なし|ワークシートを保護します。ワークシートが保護されている場合はスローします。|
|[保護を解除](../api/worksheetprotection_unprotect.md)|なし|ワークシートの保護を解除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|options|[WorkbookWorksheetProtectionOptions](worksheetprotectionoptions.md)|シートの保護のオプション。読み取り専用。|
|protected|boolean|ワークシートが保護されているかどうかを示します。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
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