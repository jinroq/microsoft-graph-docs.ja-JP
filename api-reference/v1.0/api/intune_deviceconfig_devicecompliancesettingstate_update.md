# <a name="update-devicecompliancesettingstate"></a>deviceComplianceSettingState の更新

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|承認|ベアラー &lt;トークン&gt; が必須。|
|承諾|アプリケーションまたは json|

## <a name="request-body"></a>要求本文
要求本文で、[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトの JSON 表記を指定します。

次の表に、[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー|
|setting|文字列|設定のクラス名とプロパティ名。|
|settingName|文字列|レポートされている設定名。|
|deviceId|文字列|レポートされているデバイス ID。|
|deviceName|文字列|レポートされているデバイス名。|
|userId|文字列|レポートされているユーザー ID|
|userEmail|文字列|レポートされているユーザーのメール アドレス。|
|userName|文字列|レポートされているユーザー名|
|userPrincipalName|文字列|レポートされているユーザーの PrincipalName|
|deviceModel|文字列|レポートされているデバイス モデル|
|state|[complianceStatus](../resources/intune_shared_compliancestatus.md)|設定のコンプライアンスの状態です。 使用可能な値は`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が過ぎる DateTime|



## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトを応答本文で返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 450

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```








