---
title: ioseasemailprofileconfiguration リソースの種類
description: このプロファイルに構成を提供することで、iOS デバイス上のネイティブ電子メールクライアントに Exchange サーバーと通信し、電子メール、連絡先、予定表、アラーム、およびメモを取得することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f9daf2272da7c0d8b7b2c8f47ff0e7c5f8d136f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563862"
---
# <a name="ioseasemailprofileconfiguration-resource-type"></a>ioseasemailprofileconfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することで、iOS デバイス上のネイティブ電子メールクライアントに Exchange サーバーと通信し、電子メール、連絡先、予定表、アラーム、およびメモを取得することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。


[easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ioseasemailprofileconfiguraseを一覧表示する](../api/intune-deviceconfig-ioseasemailprofileconfiguration-list.md)|[ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)コレクション|[ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)プロパティオブジェクトのプロパティとリレーションシップをリストします。|
|[ioseasemailprofileconfiguration の取得](../api/intune-deviceconfig-ioseasemailprofileconfiguration-get.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|[ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)プロパティオブジェクトのプロパティとリレーションシップを読み取ります。|
|[ioseasemailprofileconfiguration 作成](../api/intune-deviceconfig-ioseasemailprofileconfiguration-create.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|新しい[ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)このオブジェクトを作成します。|
|[ioseasemailprofileconfiguration の削除](../api/intune-deviceconfig-ioseasemailprofileconfiguration-delete.md)|なし|[ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)を削除します。|
|[ioseasemailprofileconfiguration 更新](../api/intune-deviceconfig-ioseasemailprofileconfiguration-update.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|[ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)プロパティオブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|usernameSource|[useremailsource](../resources/intune-deviceconfig-useremailsource.md)|ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。 可能な値は、`userPrincipalName`、`primarySmtpAddress` です。|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md)|メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。 可能な値は `userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。|
|userdomainnamesource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|userdomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。 可能な値は、`fullDomainName`、`netBiosDomainName` です。|
|customdomainname|String|デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。 [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。|
|accountName|String|アカウント名。|
|authenticationMethod|[easauthenticationmethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|この電子メールプロファイルの認証方法。 可能な値は、`usernameAndPassword`、`certificate` です。|
|blockmovingmessagestooruncommand/電子メールアカウント|Boolean|他の電子メールアカウントへのメッセージの移動をブロックするかどうかを示します。|
|blockSendingEmailFromThirdPartyApps|Boolean|サードパーティ製アプリからの電子メールの送信をブロックするかどうかを示します。|
|blockSyncingRecentlyUsedEmailAddresses|Boolean|最近使用した電子メールアドレスの同期をブロックするかどうかを示します (たとえば、新しい電子メールを作成する場合)。|
|durationOfEmailToSync|[emailsyncduration](../resources/intune-deviceconfig-emailsyncduration.md)|電子メールを同期する時間。 . 可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。|
|emailaddresssource|[useremailsource](../resources/intune-deviceconfig-useremailsource.md)|AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。 可能な値は、`userPrincipalName`、`primarySmtpAddress` です。|
|hostName|String|ネイティブメールアプリが接続する Exchange の場所 (URL)。|
|requireSmime|Boolean|S/MIME 証明書を使用するかどうかを示します。|
|smimeEnablePerMessageSwitch|Boolean|暗号化されていない電子メールを許可するかどうかを示します。|
|smimeEncryptByDefaultEnabled|Boolean|true S/MIME 暗号化に設定すると、既定で有効になります。|
|smimeSigningEnabled|Boolean|このアカウントに対して true S/MIME 署名を有効に設定した場合|
|smimeSigningUserOverrideEnabled|Boolean|true に設定されている場合、ユーザーは S/MIME の署名のオンとオフを切り替えることができます。|
|smimeEncryptByDefaultUserOverrideEnabled|Boolean|true に設定されている場合、ユーザーは既定の設定で暗号化を切り替えることができます。|
|smimeSigningCertificateUserOverrideEnabled|Boolean|true に設定されている場合、ユーザーは署名 id を選択できます。|
|smimeEncryptionCertificateUserOverrideEnabled|Boolean|true に設定されている場合、ユーザーは S/MIME 暗号化 id を選択できます。 |
|requireSsl|Boolean|SSL を使用するかどうかを示します。|
|useoauth|Boolean|接続で認証に OAuth を使用するかどうかを指定します。|

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
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|id 証明書。|
|smimeSigningCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|S/MIME 署名証明書。|
|smimeEncryptionCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|S/MIME 暗号化証明書。|

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
  "useOAuth": true
}
```





