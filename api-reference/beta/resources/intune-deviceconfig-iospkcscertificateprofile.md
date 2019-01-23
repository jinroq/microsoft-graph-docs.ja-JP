---
title: iosPkcsCertificateProfile リソースの種類
description: iOS PKCS の証明書プロファイルです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd4c009949edadc2646a474f417b984d4700924d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401118"
---
# <a name="iospkcscertificateprofile-resource-type"></a>iosPkcsCertificateProfile リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS PKCS の証明書プロファイルです。


[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosPkcsCertificateProfiles](../api/intune-deviceconfig-iospkcscertificateprofile-list.md)|[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)コレクション|[IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトのプロパティと関係を一覧表示します。|
|[IosPkcsCertificateProfile を取得します。](../api/intune-deviceconfig-iospkcscertificateprofile-get.md)|[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)|[IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[IosPkcsCertificateProfile を作成します。](../api/intune-deviceconfig-iospkcscertificateprofile-create.md)|[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)|新しい[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトを作成します。|
|[IosPkcsCertificateProfile を削除します。](../api/intune-deviceconfig-iospkcscertificateprofile-delete.md)|なし|の[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)を削除します。|
|[IosPkcsCertificateProfile を更新します。](../api/intune-deviceconfig-iospkcscertificateprofile-update.md)|[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)|[IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|renewalThresholdPercentage|Int32|証明書の書き換えのしきい値の割合です。 有効な値は[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)からの 1 から 99 までの継承|
|subjectNameFormat|[appleSubjectNameFormat](../resources/intune-deviceconfig-applesubjectnameformat.md)|証明書のサブジェクト名の形式です。 [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。 使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|証明書のサブジェクトの別名の種類です。 [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。 可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。|
|certificateValidityPeriodValue|Int32|証明書の有効期間の値です。 [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されました。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|証明書の有効期間のスケールです。 [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承されます。 可能な値は、`days`、`months`、`years` です。|
|certificationAuthority|String|PKCS 証明機関。|
|certificationAuthorityName|String|PKCS 証明機関の名前です。|
|certificateTemplateName|String|PKCS の証明書テンプレートの名前です。|
|subjectAlternativeNameFormatString|String|AAD の属性を定義するカスタム文字列。|

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
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)コレクション|デバイスの証明書の状態|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosPkcsCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  "renewalThresholdPercentage": 1024,
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "subjectAlternativeNameFormatString": "String"
}
```




