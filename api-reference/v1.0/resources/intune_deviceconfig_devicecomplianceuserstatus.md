# <a name="devicecomplianceuserstatus-resource-type"></a>deviceComplianceUserStatus リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceComplianceUserStatuses のリスト](../api/intune_deviceconfig_devicecomplianceuserstatus_list.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) コレクション|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceComplianceUserStatus の取得](../api/intune_deviceconfig_devicecomplianceuserstatus_get.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceComplianceUserStatus の作成](../api/intune_deviceconfig_devicecomplianceuserstatus_create.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|新しい [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) オブジェクトを作成します。|
|[deviceComplianceUserStatus の削除](../api/intune_deviceconfig_devicecomplianceuserstatus_delete.md)|なし|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) を削除します。|
|[deviceComplianceUserStatus の更新](../api/intune_deviceconfig_devicecomplianceuserstatus_update.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userDisplayName|String|DevicePolicyStatus のユーザー名です。|
|devicesCount|Int32|そのユーザーのデバイスの数です。|
|status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|ポリシー レポートのコンプライアンスの状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|lastReportedDateTime|DateTimeOffset|ポリシー レポートの最終変更日時です。|
|userPrincipalName|String|UserPrincipalName。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



