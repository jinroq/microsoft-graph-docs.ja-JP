# <a name="applepushnotificationcertificate-resource-type"></a>applePushNotificationCertificate リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Apple プッシュ通知証明書。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[applePushNotificationCertificate の取得](../api/intune_devices_applepushnotificationcertificate_get.md)|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[applePushNotificationCertificate の更新](../api/intune_devices_applepushnotificationcertificate_update.md)|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。|
|[downloadApplePushNotificationCertificateSigningRequest 関数](../api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md)|文字列|Apple プッシュ通知の証明書署名要求をダウンロードします|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|証明書の一意識別子|
|appleIdentifier|文字列|MDM プッシュ証明書の作成に使用するアカウントの Apple ID。|
|topicIdentifier|文字列|トピック ID。|
|lastModifiedDateTime|DateTimeOffset|Apple プッシュ通知証明書の最終変更日時。|
|expirationDateTime|DateTimeOffset|Apple プッシュ通知証明書の有効期限。|
|証明書|文字列|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



