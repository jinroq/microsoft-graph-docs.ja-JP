---
title: Androide Asemailprofil/リソースの種類
description: このプロファイルに構成を提供することにより、Exchange サーバーと通信し、電子メール、連絡先、予定表、タスク、およびメモを取得するように、KNOX デバイス上のネイティブ電子メールクライアントに指示することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e7da685d6402e6e23728f6ac57387c74dc92b765
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971432"
---
# <a name="androideasemailprofileconfiguration-resource-type"></a>Androide Asemailprofil/リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することにより、Exchange サーバーと通信し、電子メール、連絡先、予定表、タスク、およびメモを取得するように、KNOX デバイス上のネイティブ電子メールクライアントに指示することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト Androide Asemailprofileconfigウニ](../api/intune-deviceconfig-androideasemailprofileconfiguration-list.md)|[Androide Asemailprofilreplica](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)コレクション|[Androide Asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[AndroidEasEmailProfileConfiguration の取得](../api/intune-deviceconfig-androideasemailprofileconfiguration-get.md)|[Androide Asemailprofil/スキーマ](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|[Androide Asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[AndroidEasEmailProfileConfiguration 作成](../api/intune-deviceconfig-androideasemailprofileconfiguration-create.md)|[Androide Asemailprofil/スキーマ](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|[Androide Asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)新しいオブジェクトを作成します。|
|[AndroidEasEmailProfileConfiguration の削除](../api/intune-deviceconfig-androideasemailprofileconfiguration-delete.md)|None|[Androide Asemailprofilreplica](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)を削除します。|
|[AndroidEasEmailProfileConfiguration 更新](../api/intune-deviceconfig-androideasemailprofileconfiguration-update.md)|[Androide Asemailprofil/スキーマ](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|[Androide Asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|文字列コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|このポリシーの OS エディションの適用。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|このポリシーの OS バージョン適用ルール。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|Devicemanagementの信頼性ルール Devicemode|[Devicemanagementの信頼性ルール Devicemode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|このポリシーのデバイスモード適用ルール。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountName|String|ユーザーに EA (この) プロファイルの名前として表示される Exchange ActiveSync アカウント名。|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Exchange ActiveSync の認証方法。 可能な値は、`usernameAndPassword`、`certificate`、`derivedCredential` です。|
|syncCalendar|Boolean|予定表の同期を切り替えます。 False カレンダーに設定すると、デバイスで無効になります。|
|syncContacts|Boolean|連絡先の同期を切り替えます。 False に設定すると、デバイスで [連絡先] がオフになります。|
|syncTasks|Boolean|タスクの同期を切り替えます。 False タスクに設定した場合は、デバイスで無効になります。|
|syncNotes|Boolean|メモの同期を切り替えます。 False に設定すると、デバイスでは、メモがオフになります。|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|電子メールを同期する時間の長さ。 可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。 可能な値は、`userPrincipalName`、`primarySmtpAddress` です。|
|emailSyncSchedule|[emailSyncSchedule](../resources/intune-deviceconfig-emailsyncschedule.md)|電子メール同期スケジュール。 可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。|
|hostName|String|ネイティブメールアプリが接続する Exchange の場所 (URL)。|
|requireSmime|Boolean|S/MIME 証明書を使用するかどうかを示します。|
|requireSsl|Boolean|SSL を使用するかどうかを示します。|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 使用可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 可能な値は、`fullDomainName`、`netBiosDomainName` です。|
|customDomainName|String|デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|identityCertificate|[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|Id 証明書。|
|smimeSigningCertificate|[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|S/MIME 署名証明書。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountName": "String",
  "authenticationMethod": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "emailSyncSchedule": "String",
  "hostName": "String",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String"
}
```





