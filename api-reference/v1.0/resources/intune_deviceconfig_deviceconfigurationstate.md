# <a name="deviceconfigurationstate-resource-type"></a>deviceConfigurationState リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

指定されたデバイスのデバイス構成の状態です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceConfigurationStates のリスト](../api/intune_deviceconfig_deviceconfigurationstate_list.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) コレクション|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceConfigurationState の取得](../api/intune_deviceconfig_deviceconfigurationstate_get.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceConfigurationState の作成](../api/intune_deviceconfig_deviceconfigurationstate_create.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|新しい [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) オブジェクトを作成します。|
|[deviceConfigurationState の削除](../api/intune_deviceconfig_deviceconfigurationstate_delete.md)|なし|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) を削除します。|
|[deviceConfigurationState の更新](../api/intune_deviceconfig_deviceconfigurationstate_update.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|settingStates|[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md) コレクション|まだ文書化されていません|
|displayName|String|この policyBase のポリシーの名前|
|version|Int32|ポリシーのバージョン|
|platformType|String|ポリシーが適用されるプラットフォームの種類です。可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all` です。|
|state|String|ポリシーのコンプライアンス対応状態です。可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。|
|settingCount|Int32|ポリシーが保持する設定の数|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "String",
      "settingName": "String",
      "instanceDisplayName": "String",
      "state": "String",
      "errorCode": 1024,
      "errorDescription": "String",
      "userId": "String",
      "userName": "String",
      "userEmail": "String",
      "userPrincipalName": "String",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "String",
          "displayName": "String"
        }
      ],
      "currentValue": "String"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```



