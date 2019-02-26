---
title: androide asemailprofil/リソースの種類
description: このプロファイルに構成を提供することにより、Exchange サーバーと通信し、電子メール、連絡先、予定表、タスク、およびメモを取得するように、KNOX デバイス上のネイティブ電子メールクライアントに指示することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 497a629ee500bc522e0ab2c0eb6b7b530983b956
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175200"
---
# <a name="androideasemailprofileconfiguration-resource-type"></a>androide asemailprofil/リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することにより、Exchange サーバーと通信し、電子メール、連絡先、予定表、タスク、およびメモを取得するように、KNOX デバイス上のネイティブ電子メールクライアントに指示することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androide asemailprofileconfigウニ](../api/intune-deviceconfig-androideasemailprofileconfiguration-list.md)|[androide asemailprofilreplica](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)コレクション|[androide asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[androideasemailprofileconfiguration の取得](../api/intune-deviceconfig-androideasemailprofileconfiguration-get.md)|[androide asemailprofil/スキーマ](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|[androide asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androideasemailprofileconfiguration 作成](../api/intune-deviceconfig-androideasemailprofileconfiguration-create.md)|[androide asemailprofil/スキーマ](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|[androide asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)新しいオブジェクトを作成します。|
|[androideasemailprofileconfiguration の削除](../api/intune-deviceconfig-androideasemailprofileconfiguration-delete.md)|なし|[androide asemailprofilreplica](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)を削除します。|
|[androideasemailprofileconfiguration 更新](../api/intune-deviceconfig-androideasemailprofileconfiguration-update.md)|[androide asemailprofil/スキーマ](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|[androide asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountName|String|ユーザーに ea (この) プロファイルの名前として表示される Exchange ActiveSync アカウント名。|
|authenticationMethod|[easauthenticationmethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Exchange ActiveSync の認証方法。 使用可能な値は、`usernameAndPassword`、`certificate` です。|
|synccalendar|Boolean|予定表の同期を切り替えます。 false カレンダーに設定すると、デバイスで無効になります。|
|synccontacts|Boolean|連絡先の同期を切り替えます。 false に設定すると、デバイスで [連絡先] がオフになります。|
|synctasks|Boolean|タスクの同期を切り替えます。 false タスクに設定した場合は、デバイスで無効になります。|
|syncnotes|Boolean|メモの同期を切り替えます。 false に設定すると、デバイスでは、メモがオフになります。|
|durationOfEmailToSync|[emailsyncduration](../resources/intune-deviceconfig-emailsyncduration.md)|電子メールを同期する時間の長さ。 可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。|
|emailaddresssource|[useremailsource](../resources/intune-deviceconfig-useremailsource.md)|AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。 使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。|
|emailsyncschedule|[emailsyncschedule](../resources/intune-deviceconfig-emailsyncschedule.md)|電子メール同期スケジュール。 可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。|
|hostName|String|ネイティブメールアプリが接続する Exchange の場所 (URL)。|
|requireSmime|Boolean|S/MIME 証明書を使用するかどうかを示します。|
|requireSsl|Boolean|SSL を使用するかどうかを示します。|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 使用可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。|
|userdomainnamesource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|userdomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 使用可能な値は、`fullDomainName`、`netBiosDomainName` です。|
|customdomainname|String|デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。|

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
|identityCertificate|[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|id 証明書。|
|smimeSigningCertificate|[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|S/MIME 署名証明書。|

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




