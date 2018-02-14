# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceManagement](../api/intune_devices_devicemanagement_get.md)|[deviceManagement](../resources/intune_devices_devicemanagement.md)|[deviceManagement](../resources/intune_devices_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceManagement](../api/intune_devices_devicemanagement_update.md)|[deviceManagement](../resources/intune_devices_devicemanagement.md)|[deviceManagement](../resources/intune_devices_devicemanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|デバイスの一意識別子|
|subscriptionState|文字列型 (String)|テナントのモバイル デバイス管理のサブスクリプション状態。 可能な値: `pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Apple プッシュ通知証明書。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|デバイスの概要|
|detectedApps|[detectedApp](../resources/intune_devices_detectedapp.md) コレクション|デバイスに関連付けられている、検出されたアプリの一覧。|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md) コレクション|管理対象デバイスの一覧。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



