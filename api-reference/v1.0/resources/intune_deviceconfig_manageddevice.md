# <a name="manageddevice-resource-type"></a>managedDevice リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune 経由で管理または事前登録されるデバイス
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List managedDevices](../api/intune_deviceconfig_manageddevice_list.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md) コレクション|[managedDevice](../resources/intune_deviceconfig_manageddevice.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedDevice](../api/intune_deviceconfig_manageddevice_get.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md) オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceConfigurationStates|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) コレクション|対象デバイスのデバイス構成の状態。|
|deviceCompliancePolicyStates|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) コレクション|対象デバイスのデバイス コンプライアンス ポリシーの状態。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



