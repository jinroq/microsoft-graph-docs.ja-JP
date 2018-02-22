# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment リソース タイプ

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List mobileAppAssignments](../api/intune_apps_mobileappassignment_list.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) コレクション|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get mobileAppAssignment](../api/intune_apps_mobileappassignment_get.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create mobileAppAssignment](../api/intune_apps_mobileappassignment_create.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|新しい [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) オブジェクトを作成します。|
|[Delete mobileAppAssignment](../api/intune_apps_mobileappassignment_delete.md)|なし|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) を削除します。|
|[Update mobileAppAssignment](../api/intune_apps_mobileappassignment_update.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|intent|String|管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)|管理者によって定義された、ターゲット グループの割り当て。|
|settings|[mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)|管理者によって定義された、ターゲットの割り当ての設定。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



