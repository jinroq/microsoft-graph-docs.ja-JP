# <a name="mobileappcategory-resource-type"></a>mobileAppCategory リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune のアプリの単一カテゴリのプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[mobileAppCategories のリスト](../api/intune_apps_mobileappcategory_list.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) コレクション|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[mobileAppCategory の取得](../api/intune_apps_mobileappcategory_get.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[mobileAppCategory の作成](../api/intune_apps_mobileappcategory_create.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|新しい [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) オブジェクトを作成します。|
|[mobileAppCategory の削除](../api/intune_apps_mobileappcategory_delete.md)|なし|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) を削除します。|
|[mobileAppCategory の更新](../api/intune_apps_mobileappcategory_update.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|displayName|文字列|アプリのカテゴリの名前。|
|lastModifiedDateTime|DateTimeOffset|mobileAppCategory が最後に変更された日時です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```



