# <a name="devicemanagement-resource-type"></a>deviceManagement リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス管理下で Android for Work 設定機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagement の取得](../api/intune_androidforwork_devicemanagement_get.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagement の更新](../api/intune_androidforwork_devicemanagement_update.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|単一の Android for Work 設定エンティティです。|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) コレクション|Android for Work アプリの構成スキーマ アイテムのエンティティです。|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) コレクション|Android for Work 登録プロファイルのエンティティです。|

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



