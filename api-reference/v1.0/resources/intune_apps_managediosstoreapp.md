# <a name="managediosstoreapp-resource-type"></a>managedIOSStoreApp リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune アプリ保護ポリシーで管理できる iOS ストア アプリのプロパティと継承されたプロパティが含まれます。

[managedApp](../resources/intune_apps_managedapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedIOSStoreApps の一覧表示](../api/intune_apps_managediosstoreapp_list.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) コレクション|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedIOSStoreApp の取得](../api/intune_apps_managediosstoreapp_get.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedIOSStoreApp の作成](../api/intune_apps_managediosstoreapp_create.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|新しい [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトを作成します。|
|[managedIOSStoreApp の削除](../api/intune_apps_managediosstoreapp_delete.md)|なし|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) を削除します。|
|[managedIOSStoreApp の更新](../api/intune_apps_managediosstoreapp_update.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|displayName|文字列|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|説明|文字列|アプリの説明。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|発行元|文字列|アプリの発行元。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|createdDateTime|DateTimeOffset|アプリが作成された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|アプリが最後に変更された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|isFeatured|ブール値|アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|privacyInformationUrl|文字列|プライバシーに関する声明の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|informationUrl|文字列|詳細情報の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|所有者|文字列|アプリの所有者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|開発者|文字列|アプリの開発者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|メモ|文字列|アプリ用のメモ。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します。 可能な値は、`notPublished`、`processing`、`published` です。|
|appAvailability|[managedAppAvailability](../resources/intune_apps_managedappavailability.md)|アプリケーションの可用性。 [managedApp](../resources/intune_apps_managedapp.md) から継承します。 可能な値は、`global`、`lineOfBusiness` です。|
|バージョン|文字列|アプリケーションのバージョン。 [managedApp](../resources/intune_apps_managedapp.md) から継承します|
|bundleId|文字列|アプリのバンドル ID。|
|appStoreUrl|文字列|Apple の AppStoreUrl。|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|このアプリを実行できる iOS アーキテクチャ。|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|サポートされているオペレーティング システムの最小の値です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|カテゴリー|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|割り当て|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSStoreApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String",
  "bundleId": "String",
  "appStoreUrl": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```








