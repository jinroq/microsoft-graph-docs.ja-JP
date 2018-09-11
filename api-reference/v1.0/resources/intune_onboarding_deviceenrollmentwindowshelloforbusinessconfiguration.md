# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>deviceEnrollmentWindowsHelloForBusinessConfiguration リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません

[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceEnrollmentWindowsHelloForBusinessConfigurations を一覧表示](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_list.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) コレクション|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceEnrollmentWindowsHelloForBusinessConfiguration を取得](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceEnrollmentWindowsHelloForBusinessConfiguration を作成](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。|
|[deviceEnrollmentWindowsHelloForBusinessConfiguration を削除](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_delete.md)|なし|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) を削除します。|
|[deviceEnrollmentWindowsHelloForBusinessConfiguration を更新](../api/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration_update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します|
|displayName|文字列|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します|
|description|文字列|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します|
|重要度|Int32|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します|
|バージョン|Int32|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します|
|pinMinimumLength|Int32|まだ文書化されていません|
|pinMaximumLength|Int32|まだ文書化されていません|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|まだ文書化されていません。可能な値は、`allowed`、`required`、`disallowed` です。|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|まだ文書化されていません。可能な値は、`allowed`、`required`、`disallowed` です。|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|まだ文書化されていません。可能な値は、`allowed`、`required`、`disallowed` です。|
|都道府県|[有効化](../resources/intune_onboarding_enablement.md)|まだ文書化されていません。可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|securityDeviceRequired|ブール値|まだ文書化されていません|
|unlockWithBiometricsEnabled|ブール値|まだ文書化されていません|
|remotePassportEnabled|ブール値|まだ文書化されていません|
|pinPreviousBlockCount|Int32|まだ文書化されていません|
|pinExpirationInDays|Int32|まだ文書化されていません|
|enhancedBiometricsState|[有効化](../resources/intune_onboarding_enablement.md)|まだ文書化されていません。可能な値は、`notConfigured`、`enabled`、`disabled` です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|割り当て|[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) からの継承|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceEnrollmentConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}-->
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








