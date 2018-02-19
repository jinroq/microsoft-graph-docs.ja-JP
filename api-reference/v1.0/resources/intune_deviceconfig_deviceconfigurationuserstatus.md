# <a name="deviceconfigurationuserstatus-resource-type"></a>deviceConfigurationUserStatus リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceConfigurationUserStatuses のリスト](../api/intune_deviceconfig_deviceconfigurationuserstatus_list.md)|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) コレクション|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceConfigurationUserStatus の取得](../api/intune_deviceconfig_deviceconfigurationuserstatus_get.md)|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceConfigurationUserStatus の作成](../api/intune_deviceconfig_deviceconfigurationuserstatus_create.md)|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|新しい [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) オブジェクトを作成します。|
|[deviceConfigurationUserStatus の削除](../api/intune_deviceconfig_deviceconfigurationuserstatus_delete.md)|なし|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) を削除します。|
|[deviceConfigurationUserStatus の更新](../api/intune_deviceconfig_deviceconfigurationuserstatus_update.md)|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userDisplayName|String|DevicePolicyStatus のユーザー名です。|
|devicesCount|Int32|そのユーザーのデバイスの数です。|
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
  "@odata.type": "microsoft.graph.deviceConfigurationUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



