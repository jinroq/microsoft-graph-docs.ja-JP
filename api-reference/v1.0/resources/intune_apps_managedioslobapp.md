# <a name="managedioslobapp-resource-type"></a>managedIOSLobApp リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理対象 iOS 基幹業務アプリのプロパティと継承されたプロパティが含まれます。

[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedIOSLobApps をリストします](../api/intune_apps_managedioslobapp_list.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) コレクション|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedIOSLobApp を取得します](../api/intune_apps_managedioslobapp_get.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedIOSLobApp を作成します](../api/intune_apps_managedioslobapp_create.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|新しい [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) オブジェクトを作成します。|
|[managedIOSLobApp を削除します](../api/intune_apps_managedioslobapp_delete.md)|なし|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) を削除します。|
|[managedIOSLobApp を更新します](../api/intune_apps_managedioslobapp_update.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|displayName|文字列|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|説明|文字列|アプリの説明。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|パブリッシャー|文字列|アプリの発行元。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|largeIcon|[MIME コンテンツ](../resources/intune_shared_mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|createdDateTime|DateTimeOffset|アプリが作成された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|アプリが最後に変更された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|isFeatured|ブール値|アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|privacyInformationUrl|文字列|プライバシーに関する声明の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|informationUrl|文字列|詳細情報の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|所有者|文字列|アプリの所有者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|開発者|文字列|アプリの開発者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|メモ|文字列|アプリ用のメモ。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。 [MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。使用可能な値は`notPublished`、`processing`、`published`です。|
|アプリケーション可用性|[アプリケーション可用性の管理](../resources/intune_apps_managedappavailability.md)|アプリケーションの可用性です。[managedApp](../resources/intune_apps_managedapp.md) から継承されます。使用可能な値は `global`、`lineOfBusiness` です。|
|バージョン|文字列|アプリケーションのバージョン。 [managedApp](../resources/intune_apps_managedapp.md) から継承します|
|committedContentVersion|文字列|内部にコミットされたコンテンツのバージョン。 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します|
|fileName|文字列|メインの Lob アプリケーションのファイル名。 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します|
|サイズ|Int64|アップロードされたすべてのファイルを含む合計サイズ。 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します|
|bundleId|文字列|ID 名。|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|このアプリを実行できる iOS アーキテクチャ。|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|該当するオペレーティング システムの最小の値です。|
|expirationDateTime|DateTimeOffset|有効期限。|
|VersionNumber|文字列|管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。|
|buildNumber|文字列|管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|カテゴリ|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|課題|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|contentVersions|[mobileAppContent](../resources/intune_apps_mobileappcontent.md) コレクション|このアプリのコンテンツのバージョンのリスト。 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedMobileLobApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSLobApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
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
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String"
}
```








