# <a name="deviceconfigurationdevicestatus-resource-type"></a>deviceConfigurationDeviceStatus リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceConfigurationDeviceStatuses のリスト](../api/intune_deviceconfig_deviceconfigurationdevicestatus_list.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) コレクション|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceConfigurationDeviceStatus の取得](../api/intune_deviceconfig_deviceconfigurationdevicestatus_get.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceConfigurationDeviceStatus の作成](../api/intune_deviceconfig_deviceconfigurationdevicestatus_create.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|新しい [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) オブジェクトを作成します。|
|[deviceConfigurationDeviceStatus の削除](../api/intune_deviceconfig_deviceconfigurationdevicestatus_delete.md)|なし|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) を削除します。|
|[deviceConfigurationDeviceStatus の更新](../api/intune_deviceconfig_deviceconfigurationdevicestatus_update.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) オブジェクトのプロパティを更新します。|

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
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
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



