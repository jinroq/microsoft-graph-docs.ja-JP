# <a name="windows10mobilecompliancepolicy-resource-type"></a>windows10MobileCompliancePolicy リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このクラスには、Windows 10 Mobile のコンプライアンス設定が含まれています。

[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windows10MobileCompliancePolicies のリスト](../api/intune_deviceconfig_windows10mobilecompliancepolicy_list.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) コレクション|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windows10MobileCompliancePolicy の取得](../api/intune_deviceconfig_windows10mobilecompliancepolicy_get.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windows10MobileCompliancePolicy の作成](../api/intune_deviceconfig_windows10mobilecompliancepolicy_create.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)|新しい [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) オブジェクトを作成します。|
|[windows10MobileCompliancePolicy の削除](../api/intune_deviceconfig_windows10mobilecompliancepolicy_delete.md)|なし|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) を削除します。|
|[windows10MobileCompliancePolicy の更新](../api/intune_deviceconfig_windows10mobilecompliancepolicy_update.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)|[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|description|String|デバイス構成について管理者が提供した説明です。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前です。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|passwordRequired|Boolean|Windows Phone デバイスのロックを解除するパスワードを要求します。|
|passwordBlockSimple|Boolean|カレンダーの同期を禁止するかどうかを指定します。|
|passwordMinimumLength|Int32|パスワードの最小文字数。 有効な値は 4 から 16 までです|
|passwordMinimumCharacterSetCount|Int32|パスワードに必要な文字セットの数。|
|passwordRequiredType|String|必要なパスワードの種類。 可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。|
|passwordPreviousPasswordBlockCount|Int32|再使用を禁止する、以前のパスワードの数。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 255 までです|
|passwordMinutesOfInactivityBeforeLock|Int32|パスワードが要求されるまでの非アクティブ時間 (分)。|
|passwordRequireToUnlockFromIdle|Boolean|アイドル デバイスのロックを解除するパスワードを要求します。|
|osMinimumVersion|String|Windows Phone の最小バージョン。|
|osMaximumVersion|String|Windows Phone の最大バージョン。|
|earlyLaunchAntiMalwareDriverEnabled|Boolean|デバイスが Wiindows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。|
|bitLockerEnabled|Boolean|デバイスが Wiindows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。|
|secureBootEnabled|Boolean|デバイスが Wiindows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。|
|codeIntegrityEnabled|Boolean|デバイスが Wiindows デバイス正常性構成証明によって正常と報告されることを要求します。|
|storageRequireEncryption|Boolean|Windows デバイス上での暗号化を要求します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) コレクション|このルールのスケジュール済みのアクションのリスト ([deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) コレクション|DeviceComplianceDeviceStatus のリストです。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|userStatuses|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) コレクション|DeviceComplianceUserStatus のリストです。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|デバイス コンプライアンスのデバイス状態の概要 ([deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|デバイス コンプライアンスのユーザー状態の概要 ([deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|コンプライアンス設定状態のデバイスの要約 ([deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承)|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) コレクション|このコンプライアンス ポリシーの割り当てのコレクションです。 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10MobileCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordExpirationDays": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



