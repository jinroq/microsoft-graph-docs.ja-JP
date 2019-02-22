---
title: androidForWorkNineWorkEasConfiguration リソースの種類
description: このプロファイルに構成を提供することで、Android 用の9作業用電子メールクライアントに、Exchange サーバーと通信し、電子メール、連絡先、予定表、タスク、およびメモを取得するように指示することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8ff45e2ace22157f7ac83ad3bc8c64e4969fedc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156995"
---
# <a name="androidforworknineworkeasconfiguration-resource-type"></a>androidForWorkNineWorkEasConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することで、Android 用の9作業用電子メールクライアントに、Exchange サーバーと通信し、電子メール、連絡先、予定表、タスク、およびメモを取得するように指示することができます。 さらに、同期する電子メールの量と、デバイスの同期頻度を指定することもできます。


[androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidForWorkNineWorkEasConfigurations](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-list.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)コレクション|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[androidForWorkNineWorkEasConfiguration を取得する](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-get.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidForWorkNineWorkEasConfiguration を作成する](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-create.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|新しい[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトを作成します。|
|[androidForWorkNineWorkEasConfiguration の削除](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-delete.md)|なし|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)を削除します。|
|[androidForWorkNineWorkEasConfiguration の更新](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-update.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|authenticationMethod|[easauthenticationmethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Exchange ActiveSync の認証方法。 [androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。 使用可能な値は、`usernameAndPassword`、`certificate` です。|
|durationOfEmailToSync|[emailsyncduration](../resources/intune-deviceconfig-emailsyncduration.md)|電子メールを同期する時間の長さ。 [androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。 可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。|
|emailaddresssource|[useremailsource](../resources/intune-deviceconfig-useremailsource.md)|AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。 [androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。 使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。|
|hostName|String|メールアプリが接続する Exchange の場所 (URL)。 [androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します|
|requireSsl|ブール値|SSL を使用するかどうかを示します。 [androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。 [androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します。 使用可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。|
|synccalendar|ブール値|予定表の同期を切り替えます。 false に設定すると、予定表はデバイスで無効になります。|
|synccontacts|ブール値|連絡先の同期を切り替えます。 false に設定すると、デバイスで [連絡先] がオフになります。|
|synctasks|ブール値|タスクの同期を切り替えます。 false タスクに設定した場合は、デバイスで無効になります。|

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
|identityCertificate|[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|id 証明書。 [androidforworkeasemailprofilebase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkNineWorkEasConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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
  "authenticationMethod": "String",
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSsl": true,
  "usernameSource": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




