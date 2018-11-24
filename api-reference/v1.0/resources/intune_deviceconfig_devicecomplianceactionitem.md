# <a name="devicecomplianceactionitem-resource-type"></a>deviceComplianceActionItem リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

スケジュール済みのアクションの構成
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceComplianceActionItems](../api/intune_deviceconfig_devicecomplianceactionitem_list.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) コレクション|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_get.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_create.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|新しい [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトを作成します。|
|[Delete deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_delete.md)|なし|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) を削除します。|
|[Update deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_update.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|gracePeriodHours|Int32|アクションが実行されるまでの待機時間。 有効な値は 0 から 8760 までです|
|actionType|[deviceComplianceActionType](../resources/intune_deviceconfig_devicecomplianceactiontype.md)|実行するアクションです。 可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification` です。|
|notificationTemplateId|String|使用する通知メッセージ テンプレート|
|notificationMessageCCList|String コレクション|この通知メッセージの CC に設定するグループ ID のリスト。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



