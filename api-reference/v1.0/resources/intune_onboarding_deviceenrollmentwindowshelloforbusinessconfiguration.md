# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>deviceEnrollmentWindowsHelloForBusinessConfiguration リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません

[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceEnrollmentWindowsHelloForBusinessConfigurations](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_list.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) コレクション|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。|
|[Delete deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_delete.md)|なし|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) を削除します。|
|[Update deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。|

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
|pinMinimumLength|Int32|まだ文書化されていません|
|pinMaximumLength|Int32|まだ文書化されていません|
|pinUppercaseCharactersUsage|文字列型 (String)|まだ文書化されていません。可能な値: `allowed`、`required`、`disallowed`。|
|pinLowercaseCharactersUsage|文字列型 (String)|まだ文書化されていません。可能な値: `allowed`、`required`、`disallowed`。|
|pinSpecialCharactersUsage|文字列型 (String)|まだ文書化されていません。可能な値: `allowed`、`required`、`disallowed`。|
|state|文字列型 (String)|まだ文書化されていません。可能な値: `notConfigured`、`enabled`、`disabled`。|
|securityDeviceRequired|ブール型 (Boolean)|まだ文書化されていません|
|unlockWithBiometricsEnabled|ブール型 (Boolean)|まだ文書化されていません|
|remotePassportEnabled|ブール型 (Boolean)|まだ文書化されていません|
|pinPreviousBlockCount|Int32|まだ文書化されていません|
|pinExpirationInDays|Int32|まだ文書化されていません|
|enhancedBiometricsState|文字列型 (String)|まだ文書化されていません。可能な値: `notConfigured`、`enabled`、`disabled`。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "state": "String",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 1024,
  "pinExpirationInDays": 1024,
  "enhancedBiometricsState": "String"
}
```



