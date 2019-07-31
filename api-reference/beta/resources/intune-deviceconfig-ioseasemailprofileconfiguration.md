---
title: iosEasEmailProfileConfiguration リソースの種類
description: このプロファイルに構成を提供することで、iOS デバイス上のネイティブ電子メールクライアントに Exchange サーバーと通信し、電子メール、連絡先、予定表、アラーム、およびメモを取得することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1df54139292a3a641c2c58bfa379c8c17087b3ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001223"
---
# <a name="ioseasemailprofileconfiguration-resource-type"></a>iosEasEmailProfileConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することで、iOS デバイス上のネイティブ電子メールクライアントに Exchange サーバーと通信し、電子メール、連絡先、予定表、アラーム、およびメモを取得することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。


[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Ioseasemailprofileconfiguraseを一覧表示する](../api/intune-deviceconfig-ioseasemailprofileconfiguration-list.md)|[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)コレクション|[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)プロパティオブジェクトのプロパティとリレーションシップをリストします。|
|[IosEasEmailProfileConfiguration の取得](../api/intune-deviceconfig-ioseasemailprofileconfiguration-get.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)プロパティオブジェクトのプロパティとリレーションシップを読み取ります。|
|[IosEasEmailProfileConfiguration 作成](../api/intune-deviceconfig-ioseasemailprofileconfiguration-create.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|新しい[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)このオブジェクトを作成します。|
|[IosEasEmailProfileConfiguration の削除](../api/intune-deviceconfig-ioseasemailprofileconfiguration-delete.md)|None|[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)を削除します。|
|[IosEasEmailProfileConfiguration 更新](../api/intune-deviceconfig-ioseasemailprofileconfiguration-update.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)プロパティオブジェクトのプロパティを更新します。|

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
|usernameSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。 可能な値は、`userPrincipalName`、`primarySmtpAddress` です。|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md)|メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。 [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。 可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。 可能な値は、`fullDomainName`、`netBiosDomainName` です。|
|customDomainName|String|デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。 [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。|
|accountName|String|アカウント名。|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|この電子メールプロファイルの認証方法。 可能な値は、`usernameAndPassword`、`certificate`、`derivedCredential` です。|
|Blockmovingmessagestooruncommand/電子メールアカウント|Boolean|他の電子メールアカウントへのメッセージの移動をブロックするかどうかを示します。|
|blockSendingEmailFromThirdPartyApps|Boolean|サードパーティ製アプリからの電子メールの送信をブロックするかどうかを示します。|
|blockSyncingRecentlyUsedEmailAddresses|Boolean|最近使用した電子メールアドレスの同期をブロックするかどうかを示します (たとえば、新しい電子メールを作成する場合)。|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|電子メールを同期する時間。 . 可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。 可能な値は、`userPrincipalName`、`primarySmtpAddress` です。|
|hostName|String|ネイティブメールアプリが接続する Exchange の場所 (URL)。|
|requireSmime|Boolean|S/MIME 証明書を使用するかどうかを示します。|
|smimeEnablePerMessageSwitch|Boolean|暗号化されていない電子メールを許可するかどうかを示します。|
|smimeEncryptByDefaultEnabled|Boolean|True S/MIME 暗号化に設定すると、既定で有効になります。|
|smimeSigningEnabled|Boolean|このアカウントに対して true S/MIME 署名を有効に設定した場合|
|smimeSigningUserOverrideEnabled|Boolean|True に設定されている場合、ユーザーは S/MIME の署名のオンとオフを切り替えることができます。|
|smimeEncryptByDefaultUserOverrideEnabled|Boolean|True に設定されている場合、ユーザーは既定の設定で暗号化を切り替えることができます。|
|smimeSigningCertificateUserOverrideEnabled|Boolean|True に設定されている場合、ユーザーは署名 id を選択できます。|
|smimeEncryptionCertificateUserOverrideEnabled|Boolean|True に設定されている場合、ユーザーは S/MIME 暗号化 id を選択できます。 |
|requireSsl|Boolean|SSL を使用するかどうかを示します。|
|useOAuth|Boolean|接続で認証に OAuth を使用するかどうかを指定します。|
|signingCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|この電子メールプロファイルの署名証明書の種類。 可能な値は、`none`、`certificate`、`derivedCredential` です。|
|encryptionCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|この電子メールプロファイルの暗号化証明書の種類。 可能な値は、`none`、`certificate`、`derivedCredential` です。|

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
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Id 証明書。|
|smimeSigningCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|S/MIME 署名証明書。|
|smimeEncryptionCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|S/MIME 暗号化証明書。|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|認証に使用される派生した資格情報のテナントレベルの設定。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
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
  "usernameSource": "String",
  "usernameAADSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String",
  "accountName": "String",
  "authenticationMethod": "String",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "String",
  "encryptionCertificateType": "String"
}
```





