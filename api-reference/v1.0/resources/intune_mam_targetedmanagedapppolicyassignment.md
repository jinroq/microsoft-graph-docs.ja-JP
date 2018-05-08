# <a name="targetedmanagedapppolicyassignment-resource-type"></a>targetedManagedAppPolicyAssignment リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

グループまたはアプリの展開の種類。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List targetedManagedAppPolicyAssignments](../api/intune_mam_targetedmanagedapppolicyassignment_list.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) コレクション|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_get.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_create.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|新しい [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) オブジェクトを作成します。|
|[Delete targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_delete.md)|なし|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) を作成します。|
|[Update targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_update.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|ID|
|ターゲット|[deviceAndAppManagementAssignmentTarget](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)|グループまたはアプリの展開の識別子|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



