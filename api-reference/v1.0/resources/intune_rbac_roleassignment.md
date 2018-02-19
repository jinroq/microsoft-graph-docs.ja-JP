# <a name="roleassignment-resource-type"></a>roleAssignment リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

役割の割り当てリソースです。 役割の割り当ては、メンバーが含まれるロール定義と範囲を結びつけます。 役割ごとに 1 つまたは複数の役割の割り当てが可能です。 カスタムおよび組み込みの役割に適用されます。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[roleAssignments のリスト](../api/intune_rbac_roleassignment_list.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md) コレクション|[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[roleAssignment の取得](../api/intune_rbac_roleassignment_get.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[roleAssignment の作成](../api/intune_rbac_roleassignment_create.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|新しい [roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトを作成します。|
|[roleAssignment の削除](../api/intune_rbac_roleassignment_delete.md)|なし|[roleAssignment](../resources/intune_rbac_roleassignment.md) を削除します。|
|[roleAssignment の更新](../api/intune_rbac_roleassignment_update.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 これは読み取り専用で、自動生成されます。|
|displayName|String|役割の割り当ての表示名またはフレンドリ名です。|
|description|String|役割の割り当ての説明です。|
|resourceScopes|String コレクション|役割のスコープ メンバーのセキュリティ グループの ID リストです。  Azure Active Directory の ID です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune_rbac_roledefinition.md)|この割り当てが含まれる役割の定義。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



