# <a name="user-resource-type"></a>user リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List users](../api/intune_troubleshooting_user_list.md)|[user](../resources/intune_troubleshooting_user.md) コレクション|[user](../resources/intune_troubleshooting_user.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get user](../api/intune_troubleshooting_user_get.md)|[user](../resources/intune_troubleshooting_user.md)|[user](../resources/intune_troubleshooting_user.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create user](../api/intune_troubleshooting_user_create.md)|[user](../resources/intune_troubleshooting_user.md)|新しい [user](../resources/intune_troubleshooting_user.md) オブジェクトを作成します。|
|[Delete user](../api/intune_troubleshooting_user_delete.md)|なし|[user](../resources/intune_troubleshooting_user.md) を削除します。|
|[Update user](../api/intune_troubleshooting_user_update.md)|[user](../resources/intune_troubleshooting_user.md)|[user](../resources/intune_troubleshooting_user.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|ユーザーの一意識別子|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) コレクション|対象ユーザーのトラブルシューティング イベントの一覧です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



