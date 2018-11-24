# <a name="detectedapp-resource-type"></a>detectedApp リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。 非管理対象アプリは、会社所有のデバイスにのみ表示されます。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[detectedApps のリスト](../api/intune_devices_detectedapp_list.md)|[detectedApp](../resources/intune_devices_detectedapp.md) コレクション|[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[detectedApp の取得](../api/intune_devices_detectedapp_get.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[detectedApp の作成](../api/intune_devices_detectedapp_create.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|新しい [detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトを作成します。|
|[detectedApp の削除](../api/intune_devices_detectedapp_delete.md)|なし|[detectedApp](../resources/intune_devices_detectedapp.md) を削除します。|
|[detectedApp の更新](../api/intune_devices_detectedapp_update.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|検出されたアプリケーションの一意識別子。 これは、アプリケーションの作成時に、Intune によって自動的に生成されます。 読み取り専用です。|
|displayName|String|検出されたアプリケーションの名前。 読み取り専用です|
|version|String|検出されたアプリケーションのバージョン。 読み取り専用です|
|sizeInByte|Int64|検出されたアプリケーションのサイズ (バイト単位)。 読み取り専用です|
|deviceCount|Int32|このアプリケーションがインストールされているデバイスの数|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md) コレクション|検出されたアプリケーションがインストールされているデバイス|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```



