# <a name="managedandroidlobapp-resource-type"></a>managedAndroidLobApp リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理対象 Android 基幹業務アプリのプロパティと継承されたプロパティが含まれます。

[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedAndroidLobApps のリスト](../api/intune_apps_managedandroidlobapp_list.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) コレクション|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedAndroidLobApp を取得する](../api/intune_apps_managedandroidlobapp_get.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedAndroidLobApp を作成する](../api/intune_apps_managedandroidlobapp_create.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|新しい [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) オブジェクトを作成します。|
|[managedAndroidLobApp を削除する](../api/intune_apps_managedandroidlobapp_delete.md)|なし|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) を削除します。|
|[managedAndroidLobApp を更新する](../api/intune_apps_managedandroidlobapp_update.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|displayName|文字列|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|説明|文字列|アプリの説明。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|パブリッシャー|文字列|アプリの発行元。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|largeIcon|[mimeコンテンツ](../resources/intune_shared_mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|作成された日時|オフセット日時|アプリが作成された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|最後に変更された日時|オフセット日時|アプリが最後に変更された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|おすすめ|ブール値|アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|プライバシー情報の URL|文字列|プライバシーに関する声明の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|詳細情報の URL|文字列|詳細情報の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|所有者|文字列|アプリの所有者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|開発者|文字列|アプリの開発者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|メモ|文字列|アプリ用のメモ。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|公開の状態|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。 [MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。使用可能な値は`notPublished`、`processing`、`published`です。|
|アプリケーション可用性|[アプリケーション可用性の管理](../resources/intune_apps_managedappavailability.md)|The Application's availability. Inherited from [managedApp](../resources/intune_apps_managedapp.md). The possible values are: `global`, `lineOfBusiness`.|
|バージョン|文字列|アプリケーションのバージョン。 [managedApp](../resources/intune_apps_managedapp.md) から継承します|
|コミットされたコンテンツのバージョン|文字列|内部にコミットされたコンテンツのバージョン。 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します|
|ファイル名|文字列|メインの Lob アプリケーションのファイル名。 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します|
|サイズ|Int64|アップロードされたすべてのファイルを含む合計サイズ。 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します|
|パッケージのId|文字列|パッケージの識別子。|
|オペレーティング システムの最小値|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|該当するオペレーティング システムの最小の値です。|
|バージョン名|文字列|管理対象 Android 基幹業務 (LoB) アプリのバージョン名。|
|バージョン コード|文字列|管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|カテゴリ|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|割り当て|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|コンテンツのバージョン|[mobileAppContent](../resources/intune_apps_mobileappcontent.md) コレクション|このアプリのコンテンツのバージョンのリスト。 [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedMobileLobApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidLobApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "packageId": "String",
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
  },
  "versionName": "String",
  "versionCode": "String"
}
```








