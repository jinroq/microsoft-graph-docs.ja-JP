# <a name="windowsmobilemsi-resource-type"></a>windowsMobileMSI リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows Mobile MSI 基幹業務アプリケーションのプロパティと継承されたプロパティが含まれます。

[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsMobileMSIs を一覧表示](../api/intune_apps_windowsmobilemsi_list.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) コレクション|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsMobileMSI を取得](../api/intune_apps_windowsmobilemsi_get.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsMobileMSI を作成](../api/intune_apps_windowsmobilemsi_create.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|新しく [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) オブジェクトを作成します。|
|[windowsMobileMSI を削除](../api/intune_apps_windowsmobilemsi_delete.md)|なし|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) を削除します。|
|[windowsMobileMSI を更新](../api/intune_apps_windowsmobilemsi_update.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
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
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることはできません。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します。 指定できる値は、 `notPublished`、`processing`、`published` です。|
|committedContentVersion|文字列|内部にコミットされたコンテンツのバージョン。 [mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します|
|fileName|文字列|メインの Lob アプリケーションのファイル名。 [mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します|
|サイズ|Int64|アップロードされたすべてのファイルを含む合計サイズ。 [mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します|
|commandLine|文字列|コマンド ライン。|
|productCode|文字列|製品コード。|
|productVersion|文字列|Windows Mobile MSI 基幹業務 (LoB) アプリの製品のバージョン。|
|ignoreVersionDetection|ブール値|アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。 自己更新機能を使用する Windows Mobile MSI 基幹業務 (LoB) アプリの場合は、true に設定します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|カテゴリー|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|割り当て|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|contentVersions|[mobileAppContent](../resources/intune_apps_mobileappcontent.md) コレクション|このアプリのコンテンツのバージョンのリスト。 [mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.mobileLobApp",
  "@odata.type": "microsoft.graph.windowsMobileMSI"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true
}
```



