# <a name="devicecompliancedevicestatus-resource-type"></a>deviceComplianceDeviceStatus リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceComplianceDeviceStatuses のリスト](../api/intune_deviceconfig_devicecompliancedevicestatus_list.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) コレクション|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceComplianceDeviceStatus の取得](../api/intune_deviceconfig_devicecompliancedevicestatus_get.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceComplianceDeviceStatus の作成](../api/intune_deviceconfig_devicecompliancedevicestatus_create.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|新しい [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) オブジェクトを作成します。|
|[deviceComplianceDeviceStatus の削除](../api/intune_deviceconfig_devicecompliancedevicestatus_delete.md)|なし|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) を削除します。|
|[deviceComplianceDeviceStatus の更新](../api/intune_deviceconfig_devicecompliancedevicestatus_update.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|deviceDisplayName|String|DevicePolicyStatus のデバイス名です。|
|userName|String|レポートされているユーザー名です|
|deviceModel|String|レポートされているデバイス モデルです|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|デバイス コンプライアンスの猶予期間が過ぎた DateTime です|
|status|String|ポリシー レポートのコンプライアンスの状態です。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。|
|lastReportedDateTime|DateTimeOffset|ポリシー レポートの最終変更日時です。|
|userPrincipalName|String|UserPrincipalName。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



