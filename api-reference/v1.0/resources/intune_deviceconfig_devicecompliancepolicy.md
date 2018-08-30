# <a name="devicecompliancepolicy-resource-type"></a>deviceCompliancePolicy リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

これは、コンプライアンス ポリシーの基本クラスです。 コンプライアンス ポリシーはプラットフォーム固有のものであり、個々のプラットフォームごとのコンプライアンス ポリシーはここから継承されます。 
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceCompliancePolicies のリスト](../api/intune_deviceconfig_devicecompliancepolicy_list.md)|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) コレクション|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceCompliancePolicy の取得](../api/intune_deviceconfig_devicecompliancepolicy_get.md)|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[割り当ての操作](../api/intune_deviceconfig_devicecompliancepolicy_assign.md)|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) コレクション|まだ文書化されていません|
|[scheduleActionsForRules action](../api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|説明|文字列|デバイス構成について管理者が提供した説明です。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。|
|displayName|文字列|デバイス構成について管理者が指定した名前です。|
|バージョン|Int32|デバイス構成のバージョン。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) コレクション|このルールのスケジュール済みのアクションのリスト|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) コレクション|DeviceComplianceDeviceStatus のリスト。|
|userStatuses|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) コレクション|DeviceComplianceUserStatus のリスト。|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|デバイス コンプライアンスとデバイス状態の概要|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|デバイス コンプライアンスとユーザー状態の概要|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|コンプライアンス設定状態のデバイスの要約|
|割り当て|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) コレクション|このコンプライアンス ポリシーの割り当てのコレクション。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



