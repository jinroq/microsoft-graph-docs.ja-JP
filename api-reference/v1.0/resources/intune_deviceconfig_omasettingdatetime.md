# <a name="omasettingdatetime-resource-type"></a>omaSettingDateTime リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

OMA 設定の DateTime の定義です。

[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|displayName|文字列|表示名。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|説明|String|説明。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|omaUri|文字列|OMA。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|値|DateTimeOffset|値。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



