# <a name="notificationmessagetemplate-resource-type"></a>notificationMessageTemplate リソース タイプ

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。 管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。 notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List notificationMessageTemplates](../api/intune_notification_notificationmessagetemplate_list.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) コレクション|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_get.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_create.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|新しい [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) を作成します。|
|[Delete notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_delete.md)|なし|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) を削除します。|
|[Update notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_update.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) オブジェクトのプロパティを更新します。|
|[sendTestMessage action](../api/intune_notification_notificationmessagetemplate_sendtestmessage.md)|なし|既定のロケールで、指定された notificationMessageTemplate を使用して、テスト メッセージを送信します|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。|
|displayName|String|通知メッセージ テンプレートの表示名。|
|DefaultLocale|String|要求されたロケールが使用できないときにフォールバックする既定のロケール。|
|brandingOptions|String|メッセージ テンプレートのブランド化オプション。 ブランド化は、Intune 管理コンソールで定義されます。 可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|localizedNotificationMessages|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) コレクション|この通知メッセージ テンプレート用にローカライズされたメッセージのリスト。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```



