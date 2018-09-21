# <a name="alerttrigger-resource-type"></a>alertTrigger リソースの種類

(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|名前|文字列|検出のトリガーとして機能するプロパティの名前です。|
|型|文字列|解釈のキーと値のペアのプロパティの型。 例えば、文字列、ブール値などです。|
|値|文字列|検出トリガーとして機能するプロパティの値です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a>例

```json
{
  "name": "endpointAddress",
  "type": "networkConnection.sourceAddress",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->