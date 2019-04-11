---
title: iosscepcertificateprofile リソースの種類
description: iOS SCEP 証明書プロファイル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0c0fbddf1fdb765c8d5ac6891db86edd6474f58
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789977"
---
# <a name="iosscepcertificateprofile-resource-type"></a>iosscepcertificateprofile リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS SCEP 証明書プロファイル。


[ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosscepcertificateprofiles のリスト](../api/intune-deviceconfig-iosscepcertificateprofile-list.md)|[iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)コレクション|[iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[iosscepcertificateprofile の取得](../api/intune-deviceconfig-iosscepcertificateprofile-get.md)|[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)|[iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosscepcertificateprofile の作成](../api/intune-deviceconfig-iosscepcertificateprofile-create.md)|[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)|新しい[iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトを作成します。|
|[iosscepcertificateprofile の削除](../api/intune-deviceconfig-iosscepcertificateprofile-delete.md)|なし|[iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)を削除します。|
|[iosscepcertificateprofile の更新](../api/intune-deviceconfig-iosscepcertificateprofile-update.md)|[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)|[iosscepcertificateprofile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|renewalThresholdPercentage|Int32|証明書の更新しきい値の割合。 有効な値は、 [ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承された値 1 ~ 99 です。|
|subjectNameFormat|[appleSubjectNameFormat](../resources/intune-deviceconfig-applesubjectnameformat.md)|証明書のサブジェクト名の形式。 [ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。 可能な値は `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber` です。|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|証明書のサブジェクトの別名の種類。 [ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。 可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。|
|certificateValidityPeriodValue|Int32|証明書の有効期間の値。 [ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|証明書の有効期間のスケール。 [ioscertificateprofilebase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)から継承します。 使用可能な値は、`days`、`months`、`years` です。|
|scepServerUrls|String コレクション|SCEP サーバーの Url。|
|subjectnameformatstring プロパティ|文字列|SubjectNameFormat = custom で使用するカスタム形式。 例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US|
|keyusage|[keyusages](../resources/intune-deviceconfig-keyusages.md)|SCEP キーの使用法。 可能な値は、`keyEncipherment`、`digitalSignature` です。|
|keySize|[keySize](../resources/intune-deviceconfig-keysize.md)|SCEP キーのサイズ。 可能な値は、`size1024`、`size2048` です。|
|extendedkeyusages|[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション|拡張キー使用法 (EKU) の設定。 このコレクションには、最大で 500 個の要素を含めることができます。|
|subjectAlternativeNameFormatString|文字列|AAD 属性を定義するカスタム文字列。|
|certificateStore|[certificateStore](../resources/intune-deviceconfig-certificatestore.md)|ターゲットストアの証明書。 可能な値は、`user`、`machine` です。|
|customSubjectAlternativeNames|[customsubject代替 (ベンダー](../resources/intune-deviceconfig-customsubjectalternativename.md) ) コレクション|カスタムサブジェクトの別名設定。 このコレクションには、最大で 500 個の要素を含めることができます。|

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
|rootcertificate|[iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md)|信頼されたルート証明書。|
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)コレクション|デバイスの証明書の状態|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosScepCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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
  "scepServerUrls": [
    "String"
  ],
  "subjectNameFormatString": "String",
  "keyUsage": "String",
  "keySize": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "subjectAlternativeNameFormatString": "String",
  "certificateStore": "String",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "String",
      "name": "String"
    }
  ]
}
```





