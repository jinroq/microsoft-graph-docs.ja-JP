# <a name="devicecategory-resource-type"></a>deviceCategory リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス カテゴリは、デバイスを整理する方法を提供します。 デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。 これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceCategories のリスト](../api/intune_onboarding_devicecategory_list.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md) コレクション|[deviceCategory](../resources/intune_onboarding_devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceCategory の取得](../api/intune_onboarding_devicecategory_get.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md) オブジェクトのプロパティと関係を読み取ります。|
|[deviceCategory の作成](../api/intune_onboarding_devicecategory_create.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|新しい [deviceCategory](../resources/intune_onboarding_devicecategory.md) オブジェクトを作成します。|
|[deviceCategory の削除](../api/intune_onboarding_devicecategory_delete.md)|なし|[deviceCategory](../resources/intune_onboarding_devicecategory.md) を削除します。|
|[deviceCategory の更新](../api/intune_onboarding_devicecategory_update.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイス カテゴリの一意識別子。 読み取り専用です。|
|displayName|String|デバイス カテゴリの表示名。|
|description|String|デバイス カテゴリに関するオプションの説明。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



