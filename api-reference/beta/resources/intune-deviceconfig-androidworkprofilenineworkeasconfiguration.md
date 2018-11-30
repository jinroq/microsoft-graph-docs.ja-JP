---
title: androidWorkProfileNineWorkEasConfiguration リソースの種類
description: このプロファイルの構成を提供することによって作業 9 電子メール クライアントを Exchange サーバーと通信し、電子メール、連絡先、カレンダー、タスク、およびメモを取得する作業プロファイルの Android デバイス上に指示できます。 さらに、同期とデバイスを同期する必要がありますどのくらいの頻度にどのくらいのメールを指定することもできます。
ms.openlocfilehash: a818dc406bf1679f8bfcff0d943a2da7c5291937
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073252"
---
# <a name="androidworkprofilenineworkeasconfiguration-resource-type"></a>androidWorkProfileNineWorkEasConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このプロファイルの構成を提供することによって作業 9 電子メール クライアントを Exchange サーバーと通信し、電子メール、連絡先、カレンダー、タスク、およびメモを取得する作業プロファイルの Android デバイス上に指示できます。 さらに、同期とデバイスを同期する必要がありますどのくらいの頻度にどのくらいのメールを指定することもできます。

[AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidWorkProfileNineWorkEasConfigurations](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-list.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)コレクション|[AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[AndroidWorkProfileNineWorkEasConfiguration を取得します。](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-get.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|[AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[AndroidWorkProfileNineWorkEasConfiguration を作成します。](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-create.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|新しい[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトを作成します。|
|[AndroidWorkProfileNineWorkEasConfiguration を削除します。](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-delete.md)|なし|の[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)を削除します。|
|[AndroidWorkProfileNineWorkEasConfiguration を更新します。](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-update.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|[AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは値の取得のみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Exchange ActiveSync の認証方法です。 [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。 使用可能な値は、`usernameAndPassword`、`certificate` です。|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|電子メールの時間の期間に同期する必要があります。 [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。 可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたメール属性です。 [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。 使用可能な値は、`userPrincipalName`、`primarySmtpAddress` です。|
|hostName|String|Exchange の場所 (URL)、メール ・ アプリケーションに接続します。 [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。|
|requireSsl|ブール値|SSL を使用するかどうかを示します。 [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|AAD から選択され、デバイスにインストールする前に、このプロファイルに挿入されたユーザー名の属性です。 [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されます。 可能な値は、`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress` です。|
|syncCalendar|ブール値|カレンダーの同期を切り替えます。 場合は、デバイス上の予定表を false に設定がオフになっているとなります。|
|syncContacts|ブール値|連絡先の同期を切り替えます。 場合は取引先担当者の場合は false に設定は、デバイスの電源が切れます。|
|syncTasks|ブール値|タスクの同期を切り替えます。 場合はタスクの場合は false に設定は、デバイスの電源が切れます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|identityCertificate|[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)|Id の証明書です。 [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileNineWorkEasConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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





