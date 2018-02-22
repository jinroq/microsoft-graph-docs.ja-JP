# <a name="manageddevice-resource-type"></a>managedDevice リソース タイプ

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune 経由で管理または事前登録されるデバイス
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List managedDevices](../api/intune_devices_manageddevice_list.md)|[managedDevice](../resources/intune_devices_manageddevice.md) コレクション|[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedDevice](../api/intune_devices_manageddevice_get.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create managedDevice](../api/intune_devices_manageddevice_create.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|新しい [managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトを作成します。|
|[Delete managedDevice](../api/intune_devices_manageddevice_delete.md)|なし|[managedDevice](../resources/intune_devices_manageddevice.md) を削除します。|
|[Update managedDevice](../api/intune_devices_manageddevice_update.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|[managedDevice](../resources/intune_devices_manageddevice.md) オブジェクトのプロパティを更新します。|
|[retire action](../api/intune_devices_manageddevice_retire.md)|なし|デバイスを破棄します|
|[wipe action](../api/intune_devices_manageddevice_wipe.md)|なし|デバイスをワイプします|
|[resetPasscode action](../api/intune_devices_manageddevice_resetpasscode.md)|なし|パスコードをリセットします|
|[remoteLock action](../api/intune_devices_manageddevice_remotelock.md)|なし|リモート ロック|
|[requestRemoteAssistance action](../api/intune_devices_manageddevice_requestremoteassistance.md)|なし|リモート アシスタンスを要求します|
|[disableLostMode action](../api/intune_devices_manageddevice_disablelostmode.md)|なし|紛失モードを無効化します|
|[locateDevice action](../api/intune_devices_manageddevice_locatedevice.md)|なし|デバイスを検索します|
|[bypassActivationLock action](../api/intune_devices_manageddevice_bypassactivationlock.md)|なし|アクティベーション ロックをバイパスします|
|[rebootNow action](../api/intune_devices_manageddevice_rebootnow.md)|なし|デバイスを再起動します|
|[shutDown action](../api/intune_devices_manageddevice_shutdown.md)|なし|デバイスをシャットダウンします|
|[recoverPasscode action](../api/intune_devices_manageddevice_recoverpasscode.md)|なし|パスコードを回復します|
|[cleanWindowsDevice action](../api/intune_devices_manageddevice_cleanwindowsdevice.md)|なし|Windows デバイスをクリーンにします|
|[logoutSharedAppleDeviceActiveUser action](../api/intune_devices_manageddevice_logoutsharedappledeviceactiveuser.md)|なし|共有の Apple デバイスのアクティブなユーザーをログアウトします|
|[deleteUserFromSharedAppleDevice action](../api/intune_devices_manageddevice_deleteuserfromsharedappledevice.md)|なし|共有の Apple デバイスからユーザーを削除します|
|[syncDevice action](../api/intune_devices_manageddevice_syncdevice.md)|なし|まだ文書化されていません|
|[windowsDefenderScan action](../api/intune_devices_manageddevice_windowsdefenderscan.md)|なし|まだ文書化されていません|
|[windowsDefenderUpdateSignatures action](../api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md)|なし|まだ文書化されていません|
|[updateWindowsDeviceAccount action](../api/intune_devices_manageddevice_updatewindowsdeviceaccount.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスの一意識別子|
|userId|String|デバイスに関連付けられているユーザーの一意の識別子|
|deviceName|String|デバイスの名前|
|deviceActionResults|[deviceActionResult](../resources/intune_devices_deviceactionresult.md) コレクション|ComplexType deviceActionResult オブジェクトのリスト。|
|enrolledDateTime|DateTimeOffset|デバイスの登録時刻。|
|lastSyncDateTime|DateTimeOffset|デバイスが Intune との正常な同期を最終的に完了した日時。|
|operatingSystem|String|デバイスのオペレーティング システム。 Windows、iOS など。|
|complianceState|String|デバイスのコンプライアンス状態。 可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。|
|jailBroken|String|デバイスが脱獄またはルート化されたかどうかを示します。|
|managementAgent|String|デバイスの管理チャネル。 Intune、EAS など。可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController` です。|
|osVersion|String|デバイスのオペレーティング システムのバージョン。|
|easActivated|Boolean|Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。|
|easDeviceId|String|デバイスの Exchange ActiveSync の ID。|
|easActivationDateTime|DateTimeOffset|デバイスの Exchange ActivationSync のアクティブ化の時刻。|
|azureADRegistered|Boolean|Azure Active Directory が登録されているデバイスかどうかを示します。|
|deviceEnrollmentType|String|デバイスの登録の種類。 可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。|
|activationLockBypassCode|String|デバイスのアクティベーション ロックをバイパスするためのコード。|
|emailAddress|String|デバイスに関連付けられているユーザーの電子メール|
|azureADDeviceId|String|Azure Active Directory デバイスの一意識別子。 読み取り専用。|
|deviceRegistrationState|String|デバイスの登録状態。 可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。|
|deviceCategoryDisplayName|String|デバイス カテゴリの表示名|
|isSupervised|Boolean|デバイスの管理状況|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|最後にデバイスが Exchange に接続した時刻。|
|exchangeAccessState|String|Exchange でのデバイスのアクセスの状態。 可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。|
|exchangeAccessStateReason|String|Exchange でのデバイスの状態の理由。 可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。|
|remoteAssistanceSessionUrl|String|デバイスとのリモート アシスタンス セッションを確立できるようにする URL。|
|remoteAssistanceSessionErrorDetails|String|リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。|
|isEncrypted|Boolean|デバイスの暗号化の状態|
|userPrincipalName|String|デバイスのユーザー プリンシパル名。|
|model|String|デバイスのモデル|
|manufacturer|String|デバイスのメーカー|
|imei|String|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が過ぎる DateTime|
|serialNumber|String|SerialNumber|
|phoneNumber|String|デバイスの電話番号|
|androidSecurityPatchLevel|String|Android セキュリティ パッチのレベル|
|userDisplayName|String|ユーザーの表示名|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|ConfigrMgr クライアントが有効になっている機能|
|wiFiMacAddress|String|Wi-fi MAC|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune_devices_devicehealthattestationstate.md)|デバイスの正常性構成証明の状態。|
|subscriberCarrier|String|サブスクライバー通信事業者|
|meid|String|MEID|
|totalStorageSpaceInBytes|Int64|記憶域の合計 (バイト)|
|freeStorageSpaceInBytes|Int64|空き記憶域 (バイト)|
|managedDeviceName|String|デバイスを識別する名前が自動的に生成されます。 ユーザー フレンドリ名に上書きできます。|
|partnerReportedThreatState|String|Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。 読み取り専用。 可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive` です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune_devices_devicecategory.md)|デバイス カテゴリ|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
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



