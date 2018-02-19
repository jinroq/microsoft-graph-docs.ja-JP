# <a name="mobileapp-resource-type"></a>mobileApp リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune モバイル アプリの基本プロパティを含む抽象クラスです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[mobileApps のリスト](../api/intune_apps_mobileapp_list.md)|[mobileApp](../resources/intune_apps_mobileapp.md) コレクション|[mobileApp](../resources/intune_apps_mobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[MobileApp の取得](../api/intune_apps_mobileapp_get.md)|[mobileApp](../resources/intune_apps_mobileapp.md)|[mobileApp](../resources/intune_apps_mobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[アクションの割り当て](../api/intune_apps_mobileapp_assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|displayName|String|管理者が提供またはインポートしたアプリのタイトルです。|
|description|String|アプリの説明。|
|publisher|String|アプリの発行元。|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。|
|createdDateTime|DateTimeOffset|アプリが作成された日時。|
|lastModifiedDateTime|DateTimeOffset|アプリが最後に変更された日時。|
|isFeatured|Boolean|アプリが管理者のおすすめとしてマークされたかどうかを示す値。|
|privacyInformationUrl|String|プライバシーに関する声明の URL。|
|informationUrl|String|詳細情報の URL。|
|owner|String|アプリの所有者。|
|developer|String|アプリの開発者。|
|notes|String|アプリ用のメモ。|
|publishingState|String|アプリの発行の状態。 アプリが発行されていない限り、アプリを割り当てることができません。 可能な値は、`notPublished`、`processing`、`published` です。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|このアプリのカテゴリのリストです。|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) コレクション|このモバイル アプリのグループ割り当てのリスト。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  "publishingState": "String"
}
```



