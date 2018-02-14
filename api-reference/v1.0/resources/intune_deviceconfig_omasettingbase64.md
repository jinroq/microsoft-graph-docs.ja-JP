# <a name="omasettingbase64-resource-type"></a>omaSettingBase64 リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

OMA 設定の Base64 定義。

[omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列型 (String)|表示名。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|description|文字列型 (String)|説明。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|omaUri|文字列型 (String)|OMA。 [omaSetting](../resources/intune_deviceconfig_omasetting.md) からの継承|
|fileName|文字列型 (String)|Value プロパティに関連付けられているファイル名 (*.cer | *.crt )。|
|value|文字列型 (String)|値。 (Base64 エンコード文字列)|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



