# <a name="omasettingfloatingpoint-resource-type"></a>omaSettingFloatingPoint リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

OMA 設定の浮動小数点の定義です。

[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列|表示名。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|説明|文字列|説明。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|omaUri|文字列|OMA。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|値|単精度浮動小数点型 (Single)|値。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



