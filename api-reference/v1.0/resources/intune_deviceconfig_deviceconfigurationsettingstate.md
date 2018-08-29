# <a name="deviceconfigurationsettingstate-resource-type"></a>deviceConfigurationSettingState リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

指定されたデバイスのデバイス構成設定の状態。
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|setting|文字列|レポートされている設定値です。|
|settingName|文字列|レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です|
|instanceDisplayName|文字列|レポートされている設定インスタンスの名前です。|
|状態|[complianceStatus](../resources/intune_shared_compliancestatus.md)|設定のコンプライアンスの状態です。 指定できる値: `unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。|
|errorCode|Int64|設定のエラー コード|
|errorDescription|文字列|エラーの説明|
|userId|文字列|UserId|
|userName|文字列|UserName|
|userEmail|文字列|UserEmail|
|userPrincipalName|文字列|UserPrincipalName。|
|ソース|[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション|投稿ポリシー|
|currentValue|文字列|デバイスに関する設定の現在の値|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}-->
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



