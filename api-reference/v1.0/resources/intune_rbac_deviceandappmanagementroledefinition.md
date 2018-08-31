# <a name="deviceandappmanagementroledefinition-resource-type"></a>deviceAndAppManagementRoleDefinition リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ロールの定義リソースです。 ロールの定義は、Intune におけるロール ベース アクセスの基礎です。 ロールは、モバイル アプリなどの Intune リソースと、リソースに対する Create や Read などの関連するロールのアクセス許可を結びつけます。 ロールには、組み込みとカスタムの 2 種類があります。 組み込みのロールは変更できません。 組み込みのロールとカスタム ロールは両方とも、割り当てを実施する必要があります。 ロールを定義して、任意の使用可能なリソースとロールのアクセス許可を結合して単一のロールにしたい場合、カスタム ロールを作成します。

[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceAndAppManagementRoleDefinitions のリスト](../api/intune_rbac_deviceandappmanagementroledefinition_list.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) コレクション|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceAndAppManagementRoleDefinition の取得](../api/intune_rbac_deviceandappmanagementroledefinition_get.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceAndAppManagementRoleDefinition の作成](../api/intune_rbac_deviceandappmanagementroledefinition_create.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|新しい [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトを作成します。|
|[deviceAndAppManagementRoleDefinition の削除](../api/intune_rbac_deviceandappmanagementroledefinition_delete.md)|なし|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) の削除|
|[deviceAndAppManagementRoleDefinition の更新](../api/intune_rbac_deviceandappmanagementroledefinition_update.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 これは読み取り専用で、自動生成されます。 [roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します|
|displayName|文字列|ロールの定義の表示名。 [roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します|
|説明|文字列|ロールの定義の説明。 [roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します|
|rolePermissions|[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション|このロールに実行が許可されている、ロールのアクセス許可のリスト。 これらは、rolePermission の一部として定義されている actionName と一致する必要があります。 [roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します|
|isBuiltIn|ブール値|ロールの種類。 組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。 [roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/intune_rbac_roleassignment.md) コレクション|このロールの定義の、ロールの割り当てのリスト。 [roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.roleDefinition",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



