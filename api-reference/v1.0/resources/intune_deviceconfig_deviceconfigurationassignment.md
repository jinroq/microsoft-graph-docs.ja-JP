# <a name="deviceconfigurationassignment-resource-type"></a>deviceConfigurationAssignment リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceConfigurationAssignments のリスト](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceConfigurationAssignment の取得](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceConfigurationAssignment の作成](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|新しい [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) オブジェクトを作成します。|
|[deviceConfigurationAssignment の削除](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|なし|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) を削除します。|
|[deviceConfigurationAssignment の更新](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|割り当てのキーです。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|デバイス構成の割り当て先です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



