# <a name="deviceenrollmentlimitconfiguration-resource-type"></a>deviceEnrollmentLimitConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません

[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceEnrollmentLimitConfigurations](../api/intune_onboarding_deviceenrollmentlimitconfiguration_list.md)|[deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) コレクション|[deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceEnrollmentLimitConfiguration](../api/intune_onboarding_deviceenrollmentlimitconfiguration_get.md)|[deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)|[deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceEnrollmentLimitConfiguration](../api/intune_onboarding_deviceenrollmentlimitconfiguration_create.md)|[deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)|新しい [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。|
|[Delete deviceEnrollmentLimitConfiguration](../api/intune_onboarding_deviceenrollmentlimitconfiguration_delete.md)|なし|[deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) を削除します。|
|[Update deviceEnrollmentLimitConfiguration](../api/intune_onboarding_deviceenrollmentlimitconfiguration_update.md)|[deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)|[deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|
|displayName|文字列型 (String)|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|
|description|文字列型 (String)|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|
|priority|Int32|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|
|createdDateTime|DateTimeOffset|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|
|lastModifiedDateTime|DateTimeOffset|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|
|version|Int32|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|
|limit|Int32|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentLimitConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "limit": 1024
}
```



