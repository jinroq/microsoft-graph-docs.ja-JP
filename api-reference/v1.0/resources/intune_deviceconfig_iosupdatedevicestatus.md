# <a name="iosupdatedevicestatus-resource-type"></a>iosUpdateDeviceStatus リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosUpdateDeviceStatuses のリスト](../api/intune_deviceconfig_iosupdatedevicestatus_list.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) コレクション|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosUpdateDeviceStatus の取得](../api/intune_deviceconfig_iosupdatedevicestatus_get.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosUpdateDeviceStatus の作成](../api/intune_deviceconfig_iosupdatedevicestatus_create.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|新しい [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) オブジェクトを作成します。|
|[iosUpdateDeviceStatus の削除](../api/intune_deviceconfig_iosupdatedevicestatus_delete.md)|なし|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) を削除します。|
|[iosUpdateDeviceStatus の更新](../api/intune_deviceconfig_iosupdatedevicestatus_update.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)| [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|installStatus|[iosUpdatesInstallStatus](../resources/intune_deviceconfig_iosupdatesinstallstatus.md)|ポリシー レポートのインストール状態。 使用可能な値: `success`、 `available`、 `idle`、 `unknown`、 `downloading`、 `downloadFailed`、 `downloadRequiresComputer`、 `downloadInsufficientSpace`、 `downloadInsufficientPower`、 `downloadInsufficientNetwork`、 `installing`、 `installInsufficientSpace`、 `installInsufficientPower`、 `installPhoneCallInProgress`、 `installFailed`、 `notSupportedOperation`、 `sharedDeviceUserLoggedInError`。|
|osVersion|String|レポートされているデバイス バージョン。|
|deviceId|String|レポートされているデバイス ID。|
|userId|String|レポートされているユーザー ID。|
|deviceDisplayName|String|DevicePolicyStatus のデバイス名です。|
|userName|String|レポートされているユーザー名です|
|deviceModel|String|レポートされているデバイス モデルです|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が過ぎた DateTime です|
|status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|ポリシー レポートのコンプライアンスの状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|lastReportedDateTime|DateTimeOffset|ポリシー レポートの最終変更日時です。|
|userPrincipalName|String|UserPrincipalName。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "String (identifier)",
  "installStatus": "String",
  "osVersion": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



