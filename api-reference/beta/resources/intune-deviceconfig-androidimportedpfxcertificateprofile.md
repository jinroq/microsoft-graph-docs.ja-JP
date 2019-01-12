---
title: androidImportedPFXCertificateProfile リソースの種類
description: Android PFX インポート証明書プロファイル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7b64e968562130ad9acbb47a6f0f3971b5e99fc9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949151"
---
# <a name="androidimportedpfxcertificateprofile-resource-type"></a>androidImportedPFXCertificateProfile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android PFX インポート証明書プロファイル

[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidImportedPFXCertificateProfiles](../api/intune-deviceconfig-androidimportedpfxcertificateprofile-list.md)|[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)コレクション|[AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトのプロパティと関係を一覧表示します。|
|[AndroidImportedPFXCertificateProfile を取得します。](../api/intune-deviceconfig-androidimportedpfxcertificateprofile-get.md)|[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)|[AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[AndroidImportedPFXCertificateProfile を作成します。](../api/intune-deviceconfig-androidimportedpfxcertificateprofile-create.md)|[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)|新しい[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトを作成します。|
|[AndroidImportedPFXCertificateProfile を削除します。](../api/intune-deviceconfig-androidimportedpfxcertificateprofile-delete.md)|なし|の[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)を削除します。|
|[AndroidImportedPFXCertificateProfile を更新します。](../api/intune-deviceconfig-androidimportedpfxcertificateprofile-update.md)|[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)|[AndroidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|renewalThresholdPercentage|Int32|証明書の書き換えのしきい値の割合です。 有効な値は[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)からの 1 から 99 までの継承|
|subjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|証明書のサブジェクト名の形式です。 [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。 可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|証明書サブジェクト代替名の種類です。 [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。 可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。|
|certificateValidityPeriodValue|Int32|証明書の有効期間の値です。 [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|証明書の有効期間のスケールです。 [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。 可能な値は、`days`、`months`、`years` です。|
|extendedKeyUsages|[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション|拡張キー使用法 (EKU) 設定します。 このコレクションには、最大で 500 個の要素を含めることができます。 [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。|
|intendedPurpose|[intendedPurpose](../resources/intune-deviceconfig-intendedpurpose.md)|まだ記載されていません。 可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。|

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
|rootCertificate|[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)|信頼されたルート証明書です。 [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。|
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)コレクション|デバイスの証明書の状態|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidImportedPFXCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "intendedPurpose": "String"
}
```





