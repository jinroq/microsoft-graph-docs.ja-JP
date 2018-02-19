# <a name="devicecompliancepolicyassignment-resource-type"></a>deviceCompliancePolicyAssignment リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス コンプライアンス ポリシーの割り当てです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceCompliancePolicyAssignments のリスト](../api/intune_deviceconfig_devicecompliancepolicyassignment_list.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) コレクション|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceCompliancePolicyAssignment の取得](../api/intune_deviceconfig_devicecompliancepolicyassignment_get.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceCompliancePolicyAssignment の作成](../api/intune_deviceconfig_devicecompliancepolicyassignment_create.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|新しい [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトを作成します。|
|[deviceCompliancePolicyAssignment の削除](../api/intune_deviceconfig_devicecompliancepolicyassignment_delete.md)|なし|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) を削除します。|
|[deviceCompliancePolicyAssignment の更新](../api/intune_deviceconfig_devicecompliancepolicyassignment_update.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_deviceconfig_deviceandappmanagementassignmenttarget.md)|デバイス コンプライアンス ポリシーの割り当て先です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



