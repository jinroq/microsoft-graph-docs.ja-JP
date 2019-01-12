---
title: managedDeviceCertificateState リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 13bd57eeb37c3a35f32fd9afc57726730b4f7183
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922138"
---
# <a name="manageddevicecertificatestate-resource-type"></a>managedDeviceCertificateState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
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





