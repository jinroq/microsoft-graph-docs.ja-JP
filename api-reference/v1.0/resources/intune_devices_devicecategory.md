# <a name="devicecategory-resource-type"></a>deviceCategory リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceCategory の取得](../api/intune_devices_devicecategory_get.md)|[deviceCategory](../resources/intune_devices_devicecategory.md)|[deviceCategory](../resources/intune_devices_devicecategory.md) オブジェクトのプロパティと関係を読み取ります。|
|[deviceCategory の更新](../api/intune_devices_devicecategory_update.md)|[deviceCategory](../resources/intune_devices_devicecategory.md)|[deviceCategory](../resources/intune_devices_devicecategory.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|デバイス カテゴリの一意識別子。 読み取り専用です。|

## <a name="relationships"></a>関係
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
  "id": "String (identifier)"
}
```



