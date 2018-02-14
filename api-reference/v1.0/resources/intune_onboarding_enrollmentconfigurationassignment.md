# <a name="enrollmentconfigurationassignment-resource-type"></a>enrollmentConfigurationAssignment リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List enrollmentConfigurationAssignments](../api/intune_onboarding_enrollmentconfigurationassignment_list.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) コレクション|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_get.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_create.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|新しい [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) オブジェクトを作成します。|
|[Delete enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_delete.md)|なし|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) を削除します。|
|[Update enrollmentConfigurationAssignment](../api/intune_onboarding_enrollmentconfigurationassignment_update.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md)|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|まだ文書化されていません|
|ターゲット|[deviceAndAppManagementAssignmentTarget](../resources/intune_onboarding_deviceandappmanagementassignmenttarget.md)|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



