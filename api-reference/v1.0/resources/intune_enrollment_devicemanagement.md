# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

deviceManagement リソースは、Intune で事前設定されたテナントのコレクション デバイス ID と、事前登録構成をサポートするデバイス ID に割り当てられる登録プロファイルを表します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagement の取得](../api/intune_enrollment_devicemanagement_get.md)|[deviceManagement](../resources/intune_enrollment_devicemanagement.md)|[deviceManagement](../resources/intune_enrollment_devicemanagement.md) オブジェクトのプロパティと関係を読み取ります。|
|[deviceManagement の更新](../api/intune_enrollment_devicemanagement_update.md)|[deviceManagement](../resources/intune_enrollment_devicemanagement.md)|[deviceManagement](../resources/intune_enrollment_devicemanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|オブジェクトの GUID です。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



