# <a name="localizednotificationmessage-resource-type"></a>localizedNotificationMessage リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List localizedNotificationMessages](../api/intune_notification_localizednotificationmessage_list.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) コレクション|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_get.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_create.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|新しい [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトを作成します。|
|[Delete localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_delete.md)|なし|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) を削除します。|
|[Update localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_update.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新日時。|
|locale|文字列型 (String)|対象メッセージの送信先ロケール。|
|subject|文字列型 (String)|メッセージ テンプレートの件名。|
|messageTemplate|文字列型 (String)|メッセージ テンプレートのコンテンツ。|
|isDefault|ブール型 (Boolean)|言語フォールバック用の既定ロケールかどうかを示すフラグ。 このフラグは設定のみが可能です。 設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```



