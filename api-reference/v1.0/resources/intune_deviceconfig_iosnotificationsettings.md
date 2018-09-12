# <a name="iosnotificationsettings-resource-type"></a>iosNotificationSettings リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

通知設定を記述するアイテムです。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|bundleID|文字列|これらの通知設定を適用するアプリのバンドル ID。|
|appName|文字列|bundleID に関連するアプリケーション名。|
|publisher|文字列|bundleID に関連するパブリッシャー。|
|enabled|ブール値|通知がこのアプリで許可されているかどうかを示します。|
|showInNotificationCenter|ブール値|通知センターに通知を表示できるかどうかを示します。|
|showOnLockScreen|ブール値|ロック画面に通知を表示できるかどうかを示します。|
|alertType|[iosNotificationAlertType](../resources/intune_deviceconfig_iosnotificationalerttype.md)|このアプリの通知用の警告の種類を示します。 可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。|
|badgesEnabled|ブール値|バッジがこのアプリで許可されているかどうかを示します。|
|soundsEnabled|ブール値|サウンドがこのアプリで許可されているかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```








