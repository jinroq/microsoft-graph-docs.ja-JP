# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

deviceManagement リソースは、Intune で事前設定されたテナントのコレクション デバイス ID と、事前登録構成をサポートするデバイス ID に割り当てられる登録プロファイルを表します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceManagement](../api/intune_corpenrollment_devicemanagement_get.md)|[deviceManagement](../resources/intune_corpenrollment_devicemanagement.md)|[deviceManagement](../resources/intune_corpenrollment_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceManagement](../api/intune_corpenrollment_devicemanagement_update.md)|[deviceManagement](../resources/intune_corpenrollment_devicemanagement.md)|[deviceManagement](../resources/intune_corpenrollment_devicemanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|オブジェクトの GUID。|

## <a name="relationships"></a>リレーションシップ
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



