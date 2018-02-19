# <a name="reportroot-resource-type"></a>reportRoot リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

履歴レポートのインスタンスを表すリソースです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ReportRoot の取得](../api/intune_deviceconfig_reportroot_get.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[reportRoot の更新](../api/intune_deviceconfig_reportroot_update.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md) オブジェクトのプロパティを更新します。|
|[deviceConfigurationUserActivity function](../api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md)|[レポート](../resources/intune_deviceconfig_report.md)|デバイス構成のユーザー アクティビティ レポートのメタデータ|
|[deviceConfigurationDeviceActivity function](../api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md)|[レポート](../resources/intune_deviceconfig_report.md)|デバイス構成のデバイス アクティビティ レポートのメタデータ|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|このエンティティの一意識別子です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



