# <a name="manageddevice-resource-type"></a>managedDevice リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune 経由で管理または事前登録されるデバイス
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedDevices リスト](../api/intune_devices_manageddevice_list.md)|[managedDevice](../resources/intune_devices_manageddevice.md) コレクション|[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedDevice の取得](../api/intune_devices_manageddevice_get.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedDevice の作成](../api/intune_devices_manageddevice_create.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|新しい [managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトを作成します。|
|[managedDevice の削除](../api/intune_devices_manageddevice_delete.md)|なし|[managedDevice](../resources/intune_devices_manageddevice.md) を削除します。|
|[managedDevice の更新](../api/intune_devices_manageddevice_update.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトのプロパティを更新します。|
|[アクションを破棄します](../api/intune_devices_manageddevice_retire.md)|なし|デバイスを破棄します|
|[ワイプ操作](../api/intune_devices_manageddevice_wipe.md)|なし|デバイスをワイプします|
|[resetPasscode アクション](../api/intune_devices_manageddevice_resetpasscode.md)|なし|パスコードをリセットします|
|[remoteLock アクション](../api/intune_devices_manageddevice_remotelock.md)|なし|リモート ロック|
|[requestRemoteAssistance アクション](../api/intune_devices_manageddevice_requestremoteassistance.md)|なし|リモート アシスタンスを要求します|
|[disableLostMode アクション](../api/intune_devices_manageddevice_disablelostmode.md)|なし|紛失モードを無効化します|
|[locateDevice アクション](../api/intune_devices_manageddevice_locatedevice.md)|なし|デバイスを検索します|
|[bypassActivationLock アクション](../api/intune_devices_manageddevice_bypassactivationlock.md)|なし|アクティベーション ロックをバイパスします|
|[rebootNow アクション](../api/intune_devices_manageddevice_rebootnow.md)|なし|デバイスを再起動します|
|[shutDown アクション](../api/intune_devices_manageddevice_shutdown.md)|なし|デバイスをシャットダウンします|
|[recoverPasscode アクション](../api/intune_devices_manageddevice_recoverpasscode.md)|なし|パスコードを回復します|
|[cleanWindowsDevice アクション](../api/intune_devices_manageddevice_cleanwindowsdevice.md)|なし|Windows デバイスをクリーンにします|
|[logoutSharedAppleDeviceActiveUser アクション](../api/intune_devices_manageddevice_logoutsharedappledeviceactiveuser.md)|なし|共有の Apple デバイスのアクティブなユーザーをログアウトします|
|[deleteUserFromSharedAppleDevice アクション](../api/intune_devices_manageddevice_deleteuserfromsharedappledevice.md)|なし|共有の Apple デバイスからユーザーを削除します|
|[syncDevice アクション](../api/intune_devices_manageddevice_syncdevice.md)|なし|まだ文書化されていません|
|[windowsDefenderScan アクション](../api/intune_devices_manageddevice_windowsdefenderscan.md)|なし|まだ文書化されていません|
|[windowsDefenderUpdateSignatures アクション](../api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md)|なし|まだ文書化されていません|
|[updateWindowsDeviceAccount アクション](../api/intune_devices_manageddevice_updatewindowsdeviceaccount.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|デバイスの一意識別子|
|userId|文字列|デバイスに関連付けられているユーザーの一意の識別子|
|deviceName|文字列|デバイスの名前|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune_devices_manageddeviceownertype.md)|デバイスの所有権。 '会社' または '個人' にすることができます。 指定できる値は、`unknown`、`company`、`personal`です。|
|deviceActionResults|[deviceActionResult](../resources/intune_devices_deviceactionresult.md) コレクション|ComplexType deviceActionResult オブジェクトのリスト。|
|enrolledDateTime|DateTimeOffset|デバイスの登録時刻。|
|lastSyncDateTime|DateTimeOffset|デバイスが Intune との正常な同期を最終的に完了した日時。|
|operatingSystem|文字列|デバイスのオペレーティング システム。 Windows、iOS など。|
|complianceState|[complianceState](../resources/intune_devices_compliancestate.md)|デバイスのコンプライアンス状態。 指定できる値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。|
|jailBroken|文字列|デバイスが脱獄またはルート化されているかどうかを示します。|
|managementAgent|[managementAgentType](../resources/intune_devices_managementagenttype.md)|デバイスの管理チャネル。 Intune、EA などです。可能な値: `eas`、 `mdm`、 `easMdm`、 `intuneClient`、 `easIntuneClient`、 `configurationManagerClient`、 `configurationManagerClientMdm`、 `configurationManagerClientMdmEas`、 `unknown`、 `jamf`、 `googleCloudDevicePolicyController`。|
|osVersion|文字列|デバイスのオペレーティング システムのバージョン。|
|easActivated|ブール値|Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。|
|easDeviceId|文字列|デバイスの Exchange ActiveSync の ID。|
|easActivationDateTime|DateTimeOffset|デバイスの Exchange ActivationSync のアクティブ化の時刻。|
|azureADRegistered|ブール値|Azure Active Directory が登録されているデバイスかどうかを示します。|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune_shared_deviceenrollmenttype.md)|デバイスの登録の種類。 指定できる値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`です。|
|activationLockBypassCode|文字列|デバイスのアクティベーション ロックをバイパスするためのコード。|
|emailAddress|文字列|デバイスに関連付けられているユーザーの電子メール|
|azureADDeviceId|文字列|Azure Active Directory デバイスの一意識別子。 読み取り専用です。|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune_devices_deviceregistrationstate.md)|デバイスの登録状態。 指定できる値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`です。|
|deviceCategoryDisplayName|文字列|デバイス カテゴリの表示名|
|isSupervised|ブール値|デバイスの管理状況|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|最後にデバイスが Exchange に接続した時刻。|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|Exchange でのデバイスのアクセスの状態。 指定できる値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined`です。|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|Exchange でのデバイスのアクセス状態の理由。 指定できる値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`です。|
|remoteAssistanceSessionUrl|文字列|デバイスとのリモート アシスタンス セッションを確立できるようにする URL。|
|remoteAssistanceSessionErrorDetails|文字列|リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。|
|isEncrypted|ブール値|デバイスの暗号化の状態|
|userPrincipalName|文字列|デバイスのユーザー プリンシパル名。|
|モデル|文字列|デバイスのモデル|
|製造元|文字列|デバイスのメーカー|
|imei|文字列|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が経過する DateTime|
|serialNumber|文字列|シリアル番号|
|phoneNumber|文字列|デバイスの電話番号|
|androidSecurityPatchLevel|文字列|Android セキュリティ パッチのレベル|
|userDisplayName|文字列|ユーザーの表示名|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|ConfigrMgr クライアント対応機能|
|wiFiMacAddress|文字列|Wi-Fi MAC|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune_devices_devicehealthattestationstate.md)|デバイスの正常性構成証明の状態。|
|subscriberCarrier|文字列|サブスクライバー通信事業者|
|meid|文字列|MEID|
|totalStorageSpaceInBytes|Int64|記憶域の合計 (バイト)|
|freeStorageSpaceInBytes|Int64|空き記憶域 (バイト)|
|managedDeviceName|文字列|デバイスを識別する名前が自動的に生成されます。 ユーザー フレンドリ名に上書きできます。|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。 読み取り専用です。 指定できる値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune_shared_devicecategory.md)|デバイス カテゴリ|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedDevice"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String"
}
```



