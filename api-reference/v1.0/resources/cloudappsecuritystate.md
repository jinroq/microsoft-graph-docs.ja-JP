# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState リソースの種類

ステートフル (destinationServiceName、destinationServiceIp) は、クラウド アプリケーションについてを説明します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|destinationServiceIp|文字列|クラウド アプリケーションやサービスへの接続の宛先の IP アドレス。|
|destinationServiceName|文字列|クラウド アプリケーションとサービスの名前 (たとえば「Salesforce」、「ドロップ ボックス」など)。|
|riskScore|文字列|プロバイダーによって生成されると計算されるリスク スコア クラウド アプリケーションとサービスのです。 1 パーセンテージ相当する 0 - 1 の値の範囲を推奨します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->