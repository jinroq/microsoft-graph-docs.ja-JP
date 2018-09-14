# <a name="deviceenrollmentconfiguration-resource-type"></a>deviceEnrollmentConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceEnrollmentConfigurations のリスト](../api/intune_onboarding_deviceenrollmentconfiguration_list.md)|[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) コレクション|[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceEnrollmentConfiguration の取得](../api/intune_onboarding_deviceenrollmentconfiguration_get.md)|[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[setPriority アクション](../api/intune_onboarding_deviceenrollmentconfiguration_setpriority.md)|なし|まだ文書化されていません|
|[assign アクション](../api/intune_onboarding_deviceenrollmentconfiguration_assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|まだ文書化されていません|
|displayName|文字列|まだ文書化されていません|
|説明|文字列|まだ文書化されていません|
|優先度|Int32|まだ文書化されていません|
|createdDateTime|DateTimeOffset|まだ文書化されていません|
|lastModifiedDateTime|DateTimeOffset|まだ文書化されていません|
|バージョン|Int32|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|割り当て|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```








