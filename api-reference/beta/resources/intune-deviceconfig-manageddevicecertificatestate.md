---
title: managedDeviceCertificateState リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0975049cd7597735a32b646cc5d719b371a5d27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419101"
---
# <a name="manageddevicecertificatestate-resource-type"></a>managedDeviceCertificateState リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト managedDeviceCertificateStates](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)コレクション|[ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[ManagedDeviceCertificateState を取得します。](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|[ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトのプロパティと関係を参照してください。|
|[ManagedDeviceCertificateState を作成します。](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|新しい[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトを作成します。|
|[ManagedDeviceCertificateState を削除します。](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|なし|の[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)を削除します。|
|[ManagedDeviceCertificateState を更新します。](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|[ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|devicePlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|デバイスのプラットフォームです。 可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。|
|certificateKeyUsage|[keyUsages](../resources/intune-deviceconfig-keyusages.md)|キーの使用法です。 使用可能な値は、`keyEncipherment`、`digitalSignature` です。|
|certificateValidityPeriodUnits|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|有効期間の単位。 可能な値は、`days`、`months`、`years` です。|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|発行の状態です。 使用可能な値: `unknown`、 `challengeIssued`、 `challengeIssueFailed`、 `requestCreationFailed`、 `requestSubmitFailed`、 `challengeValidationSucceeded`、 `challengeValidationFailed`、 `issueFailed`、 `issuePending`、 `issued`、 `responseProcessingFailed`、 `responsePending`、 `enrollmentSucceeded`、 `enrollmentNotNeeded`、 `revoked`、 `removedFromCollection`、 `renewVerified`、 `installFailed`、 `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-deviceconfig-keystorageprovideroption.md)|キー記憶域プロバイダーです。 可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|サブジェクト名の形式です。 可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|サブジェクト代替名の形式です。 可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|状態を無効にします。 可能な値は、`none`、`pending`、`issued`、`failed`、`revoked` です。|
|certificateProfileDisplayName|String|証明書プロファイルの表示名|
|deviceDisplayName|String|デバイスの表示名|
|userDisplayName|String|ユーザーの表示名|
|certificateExpirationDateTime|DateTimeOffset|証明書の有効期限|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|最後の証明書の発行状態の変更|
|lastCertificateStateChangeDateTime|DateTimeOffset|最後の証明書の発行状態の変更|
|certificateIssuer|String|発行者|
|certificateThumbprint|String|拇印|
|certificateSerialNumber|String|シリアル番号|
|certificateKeyLength|Int32|キーの長さ|
|certificateEnhancedKeyUsage|String|拡張キー使用法|
|certificateValidityPeriod|Int32|有効期間|
|certificateSubjectNameFormatString|String|カスタム サブジェクト名の形式のサブジェクト名の形式の文字列|
|certificateSubjectAlternativeNameFormatString|String|カスタム書式のサブジェクト代替名の書式指定文字列|
|certificateIssuanceDateTime|DateTimeOffset|発行日|
|certificateErrorCode|Int32|エラー コード|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "String (identifier)",
  "devicePlatform": "String",
  "certificateKeyUsage": "String",
  "certificateValidityPeriodUnits": "String",
  "certificateIssuanceState": "String",
  "certificateKeyStorageProvider": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateRevokeStatus": "String",
  "certificateProfileDisplayName": "String",
  "deviceDisplayName": "String",
  "userDisplayName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateLastIssuanceStateChangedDateTime": "String (timestamp)",
  "lastCertificateStateChangeDateTime": "String (timestamp)",
  "certificateIssuer": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateKeyLength": 1024,
  "certificateEnhancedKeyUsage": "String",
  "certificateValidityPeriod": 1024,
  "certificateSubjectNameFormatString": "String",
  "certificateSubjectAlternativeNameFormatString": "String",
  "certificateIssuanceDateTime": "String (timestamp)",
  "certificateErrorCode": 1024
}
```




