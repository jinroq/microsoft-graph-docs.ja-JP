# <a name="devicemanagementpartner-resource-type"></a>deviceManagementPartner リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス管理パートナーとの接続を表すエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagementPartners をリストする](../api/intune_onboarding_devicemanagementpartner_list.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) コレクション|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceManagementPartner を取得する](../api/intune_onboarding_devicemanagementpartner_get.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagementPartner を作成する](../api/intune_onboarding_devicemanagementpartner_create.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|新しい [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトを作成します。|
|[deviceManagementPartner を削除する](../api/intune_onboarding_devicemanagementpartner_delete.md)|なし|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) を削除します。|
|[deviceManagementPartner を更新する](../api/intune_onboarding_devicemanagementpartner_update.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|まだ文書化されていません|
|lastHeartbeatDateTime|DateTimeOffset|管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|このテナントのパートナーの状態です。 指定できる値は、`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive` です。|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|パートナー アプリの種類。 指定できる値は、 `unknown`、`singleTenantApp`、`multiTenantApp` です。|
|singleTenantAppId|文字列|パートナーのシングル テナントのアプリ ID|
|displayName|文字列|パートナー表示名|
|isConfigured|ブール値|デバイス管理パートナーが構成されているかどうかを指定します|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|パートナー デバイスが削除されるときの日時 (UTC)|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|パートナー デバイスが準拠していないとマークされるときの日時 (UTC)|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```



