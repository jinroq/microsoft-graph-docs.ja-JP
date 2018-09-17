# <a name="appconfigurationsettingitem-resource-type"></a>appConfigurationSettingItem リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリの構成設定アイテムのプロパティが含まれています。
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|appConfigKey|文字列|アプリの構成キー。|
|appConfigKeyType|[mdmAppConfigKeyType](../resources/intune_apps_mdmappconfigkeytype.md)|アプリケーションの構成のキーの種類です。使用可能な値は、 `stringType`、 `integerType`、 `realType`、 `booleanType`、 `tokenType`です。|
|appConfigKeyValue|文字列|アプリの構成キーの値。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```








