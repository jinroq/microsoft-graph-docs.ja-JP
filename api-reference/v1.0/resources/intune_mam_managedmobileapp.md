# <a name="managedmobileapp-resource-type"></a>managedMobileApp リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリ展開の識別子。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List managedMobileApps](../api/intune_mam_managedmobileapp_list.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md) コレクション|[managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedMobileApp](../api/intune_mam_managedmobileapp_get.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create managedMobileApp](../api/intune_mam_managedmobileapp_create.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|新しい [managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトを作成します。|
|[Delete managedMobileApp](../api/intune_mam_managedmobileapp_delete.md)|なし|[managedMobileApp](../resources/intune_mam_managedmobileapp.md) を削除します。|
|[Update managedMobileApp](../api/intune_mam_managedmobileapp_update.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|対象のオペレーティング システムの種類のアプリの識別子。|
|id|文字列型 (String)|エンティティのキー。|
|version|文字列型 (String)|エンティティのバージョン。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



