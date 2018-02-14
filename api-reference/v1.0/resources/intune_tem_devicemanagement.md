# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceManagement](../api/intune_tem_devicemanagement_get.md)|[deviceManagement](../resources/intune_tem_devicemanagement.md)|[deviceManagement](../resources/intune_tem_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceManagement](../api/intune_tem_devicemanagement_update.md)|[deviceManagement](../resources/intune_tem_devicemanagement.md)|[deviceManagement](../resources/intune_tem_devicemanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) コレクション|通信経費の管理パートナー。|

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



