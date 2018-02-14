# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceAppManagement](../api/intune_apps_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)|[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceAppManagement](../api/intune_apps_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)|[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|mobileApps|[mobileApp](../resources/intune_apps_mobileapp.md) コレクション|モバイル アプリ。|
|mobileAppCategories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|モバイル アプリ カテゴリ。|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) コレクション|管理対象デバイスのモバイル アプリケーション構成。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



