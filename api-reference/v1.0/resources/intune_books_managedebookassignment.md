# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

グループへの電子ブックの割り当てに使用されるプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedEBookAssignments のリスト](../api/intune_books_managedebookassignment_list.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) コレクション|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedEBookAssignment の取得](../api/intune_books_managedebookassignment_get.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedEBookAssignment の作成](../api/intune_books_managedebookassignment_create.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|新しい [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトを作成します。|
|[managedEBookAssignment の削除](../api/intune_books_managedebookassignment_delete.md)|なし|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) を削除します。|
|[managedEBookAssignment の更新](../api/intune_books_managedebookassignment_update.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_books_deviceandappmanagementassignmenttarget.md)|電子ブックの割り当て先です。|
|installIntent|String|電子ブックのインストールの目的です。 可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



