# <a name="devicecompliancepolicysettingstate-resource-type"></a>deviceCompliancePolicySettingState リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|setting|文字列|レポートされている設定値です。|
|settingName|文字列|レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です|
|instanceDisplayName|文字列|レポートされている設定インスタンスの名前です。|
|state|[complianceStatus](../resources/intune_shared_compliancestatus.md)|設定のコンプライアンスの状態です。使用可能な値は `unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
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
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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








