# <a name="devicecategory-resource-type"></a>deviceCategory リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス カテゴリは、デバイスを整理する方法を提供します。 デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。 これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リストの deviceCategories](../api/intune_shared_devicecategory_list.md) コレクション|[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceCategory の取得](../api/intune_shared_devicecategory_get.md)|[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceCategory の作成](../api/intune_shared_devicecategory_create.md)|新しい [deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトを作成します。|
|[DeviceCategory を削除](../api/intune_shared_devicecategory_delete.md)。|
|[deviceCategory の更新](../api/intune_shared_devicecategory_update.md)|[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|デバイス カテゴリの一意識別子。 読み取り専用です。|
|**採用**|
|displayName|文字列|デバイス カテゴリの表示名。|
|説明|文字列|デバイス カテゴリに関するオプションの説明。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



