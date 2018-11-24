# <a name="iosvppebookassignment-resource-type"></a>iosVppEBookAssignment リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

グループへの iOS VPP 電子ブックの割り当てに使用されるプロパティが含まれています。

[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosVppEBookAssignments のリスト](../api/intune_books_iosvppebookassignment_list.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) コレクション|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosVppEBookAssignment の取得](../api/intune_books_iosvppebookassignment_get.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosVppEBookAssignment の作成](../api/intune_books_iosvppebookassignment_create.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|新しい [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) オブジェクトを作成します。|
|[iosVppEBookAssignment の削除](../api/intune_books_iosvppebookassignment_delete.md)|なし|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) を削除します。|
|[iosVppEBookAssignment の更新](../api/intune_books_iosvppebookassignment_update.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) のプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) から継承します|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|電子ブックの割り当て先。 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) から継承します|
|installIntent|[installIntent](../resources/intune_shared_installintent.md)|電子ブックのインストールの目的。 [ManagedEBookAssignment](../resources/intune_books_managedebookassignment.md)から継承されます。 可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



