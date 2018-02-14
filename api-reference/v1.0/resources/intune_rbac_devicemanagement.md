# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceManagement](../api/intune_rbac_devicemanagement_get.md)|[deviceManagement](../resources/intune_rbac_devicemanagement.md)|[deviceManagement](../resources/intune_rbac_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceManagement](../api/intune_rbac_devicemanagement_update.md)|[deviceManagement](../resources/intune_rbac_devicemanagement.md)|[deviceManagement](../resources/intune_rbac_devicemanagement.md) オブジェクトのプロパティを更新します。|
|[getEffectivePermissions 関数](../api/intune_rbac_devicemanagement_geteffectivepermissions.md)|[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション|現在の認証ユーザーの有効なアクセス許可を取得します|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|roleDefinitions|[roleDefinition](../resources/intune_rbac_roledefinition.md) コレクション|ロールの定義。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) コレクション|ロールの割り当て。|
|resourceOperations|[resourceOperation](../resources/intune_rbac_resourceoperation.md) コレクション|リソースの操作。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



