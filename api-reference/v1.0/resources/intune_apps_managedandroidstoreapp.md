# <a name="managedandroidstoreapp-resource-type"></a>managedAndroidStoreApp リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune アプリ保護ポリシーで管理できる Android ストア アプリのプロパティと継承されたプロパティが含まれます。

[managedApp](../resources/intune_apps_managedapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedAndroidStoreApps の一覧表示](../api/intune_apps_managedandroidstoreapp_list.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) コレクション|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedAndroidStoreApp の取得](../api/intune_apps_managedandroidstoreapp_get.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedAndroidStoreApp の作成](../api/intune_apps_managedandroidstoreapp_create.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|新しい [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) オブジェクトを作成します。|
|[managedAndroidStoreApp の削除](../api/intune_apps_managedandroidstoreapp_delete.md)|なし|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) を削除します。|
|[managedAndroidStoreApp の更新](../api/intune_apps_managedandroidstoreapp_update.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|displayName|文字列|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|説明|文字列|アプリの説明。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|publisher|文字列|アプリの発行元。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|createdDateTime|DateTimeOffset|アプリが作成された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|アプリが最後に変更された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|isFeatured|ブール値|アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|privacyInformationUrl|文字列|プライバシーに関する声明の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|informationUrl|文字列|詳細情報の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|owner|文字列|アプリの所有者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|developer|文字列|アプリの開発者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|notes|文字列|アプリ用のメモ。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。 [MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。使用可能な値は`notPublished`、`processing`、`published`です。|
|アプリケーション可用性|[アプリケーション可用性の管理](../resources/intune_apps_managedappavailability.md)|アプリケーションの可用性です。 [ManagedApp](../resources/intune_apps_managedapp.md)から継承されます。使用可能な値は `global`、 `lineOfBusiness`です。|
|バージョン|文字列|アプリケーションのバージョン。 [managedApp](../resources/intune_apps_managedapp.md) から継承します|
|packageId|文字列|アプリのパッケージ ID。|
|appStoreUrl|文字列|Android の AppStoreUrl。|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|サポートされているオペレーティング システムの最小の値です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|割り当て|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidStoreApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "packageId": "String",
  "appStoreUrl": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```








