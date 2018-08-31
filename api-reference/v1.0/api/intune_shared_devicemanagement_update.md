# <a name="update-devicemanagement"></a>deviceManagement の更新

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[deviceManagement](../resources/intune_shared_devicemanagement.md) オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

| アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー) | アクセス許可 (特権の大きいものから小さいものへ) |
|:---|:---|
| 委任 (職場または学校のアカウント) |
| &nbsp; &nbsp; 監査 | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; 会社の用語 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; 企業登録 | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; デバイスの構成 | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; デバイスの管理 | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; エンドポイントの保護 | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; 登録 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; 通知 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; 採用 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; RBAC | DeviceManagementRBAC.ReadWrite.All |
| &nbsp; &nbsp; リモート アシスタンス | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; 通信経費の管理パートナー | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; トラブルシューティング | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; Windows 情報保護 | DeviceManagementApps.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。|
| アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|承認|ベアラー &lt;トークン&gt; が必須。|
|承諾|アプリケーション/json|

## <a name="request-body"></a>要求本文
要求本文で、[deviceManagement](../resources/intune_shared_devicemanagement.md) オブジェクトの JSON 表記を指定します。

次の表に、[deviceManagement](../resources/intune_shared_devicemanagement.md) の作成時に必要なプロパティを示します。

|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|デバイスの一意識別子|
|**デバイスの構成**|
|設定|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|アカウント レベルの設定。|
|**デバイスの管理**|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune_devices_devicemanagementsubscriptionstate.md)|テナントのモバイル デバイス管理のサブスクリプション状態。 指定できる値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。|
|**採用**|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|intuneBrand には、ポータル サイト アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。|

要求本文のプロパティのサポートは、ワークフローによって異なります。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune_shared_devicemanagement.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a>応答

以下は、応答の例です。 注: 簡潔にするために、ここに示す応答オブジェクトは短くされている場合があります。 返されるプロパティは、ワークフローおよびコンテキストによって異なります。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```



