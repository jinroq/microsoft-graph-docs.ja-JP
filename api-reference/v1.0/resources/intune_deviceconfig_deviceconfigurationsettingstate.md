# <a name="deviceconfigurationsettingstate-resource-type"></a>deviceConfigurationSettingState リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

指定されたデバイスのデバイス構成設定の状態。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|setting|文字列型 (String)|レポートされる設定値。|
|settingName|文字列型 (String)|レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名|
|instanceDisplayName|文字列型 (String)|レポートされている設定インスタンスの名前です。|
|state|文字列型 (String)|設定のコンプライアンス対応状態です。可能な値: `unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。|
|errorCode|Int64|設定のエラー コード|
|errorDescription|文字列型 (String)|エラーの説明|
|userId|文字列型 (String)|UserId|
|userName|文字列型 (String)|UserName|
|userEmail|文字列型 (String)|UserEmail|
|userPrincipalName|文字列型 (String)|UserPrincipalName。|
|sources|[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション|投稿ポリシー|
|currentValue|文字列型 (String)|デバイスに関する設定の現在の値|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



