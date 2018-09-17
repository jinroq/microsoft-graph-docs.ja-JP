# <a name="deviceandappmanagementroleassignment-resource-type"></a>deviceAndAppManagementRoleAssignment リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みのロールに適用されます。

[roleAssignment](../resources/intune_rbac_roleassignment.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceAndAppManagementRoleAssignmentsをリストする](../api/intune_rbac_deviceandappmanagementroleassignment_list.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) コレクション|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceAndAppManagementRoleAssignmentを取得する](../api/intune_rbac_deviceandappmanagementroleassignment_get.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceAndAppManagementRoleAssignment作成する](../api/intune_rbac_deviceandappmanagementroleassignment_create.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|新しい [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトを作成します。|
|[deviceAndAppManagementRoleAssignment削除する](../api/intune_rbac_deviceandappmanagementroleassignment_delete.md)|なし|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) を削除します。|
|[deviceAndAppManagementRoleAssignmentを更新する](../api/intune_rbac_deviceandappmanagementroleassignment_update.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 これは読み取り専用で、自動生成されます。 [roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します|
|displayName|文字列|ロール割り当ての表示名またはフレンドリ名。 [roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します|
|説明|文字列|ロール割り当ての説明。 [roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します|
|resourceScopes|文字列コレクション|役割のスコープ メンバーのセキュリティ グループの ID リスト。  Azure Active Directory の ID。 [roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します|
|メンバー|文字列コレクション|ロール メンバーのセキュリティ グループの ID リスト。 Azure Active Directory の ID です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune_rbac_roledefinition.md)|対象割り当てが含まれるロール定義。 [roleAssignment](../resources/intune_rbac_roleassignment.md) からの継承|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.roleAssignment",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```








