# <a name="settingtemplatevalue-resource-type"></a>settingTemplateValue リソースの種類

設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。

### <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|defaultValue|文字列| 設定の既定値です。 |
|説明|文字列| 設定の説明です。 |
|名前|文字列| 設定の名前です。 |
|種類|文字列| 設定の種類です。 |

### <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->