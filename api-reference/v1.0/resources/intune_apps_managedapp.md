# <a name="managedapp-resource-type"></a>managedApp リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune アプリ保護ポリシーで管理できるアプリの、プロパティと継承済みプロパティを含む抽象クラス。

[mobileApp](../resources/intune_apps_mobileapp.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedApps のリスト](../api/intune_apps_managedapp_list.md)|[managedApp](../resources/intune_apps_managedapp.md) コレクション|[managedApp](../resources/intune_apps_managedapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedApp の取得](../api/intune_apps_managedapp_get.md)|[managedApp](../resources/intune_apps_managedapp.md)|[managedApp](../resources/intune_apps_managedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|displayName|String|管理者が提供またはインポートしたアプリのタイトル。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|description|String|アプリの説明。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|publisher|String|アプリの発行元。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|createdDateTime|DateTimeOffset|アプリが作成された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|アプリが最後に変更された日時。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|isFeatured|Boolean|アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|privacyInformationUrl|String|プライバシーに関する声明の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|informationUrl|String|詳細情報の URL。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|owner|String|アプリの所有者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|developer|String|アプリの開発者。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|notes|String|アプリ用のメモ。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 [MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。 可能な値は、`notPublished`、`processing`、`published` です。|
|appAvailability|[managedAppAvailability](../resources/intune_apps_managedappavailability.md)|アプリケーションの可用性。 可能な値は、`global`、`lineOfBusiness` です。|
|version|String|アプリケーションのバージョン。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|このアプリのカテゴリのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。 [mobileApp](../resources/intune_apps_mobileapp.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedApp",
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
  "version": "String"
}
```



