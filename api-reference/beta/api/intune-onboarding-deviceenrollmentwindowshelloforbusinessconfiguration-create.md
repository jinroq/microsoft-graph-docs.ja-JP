---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の作成
description: 新しい deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a566214325ec896402f7e04fff482ba0f0238bd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352890"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a>deviceEnrollmentWindowsHelloForBusinessConfiguration の作成

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトの JSON 表記を指定します。

次の表に、deviceEnrollmentWindowsHelloForBusinessConfiguration の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子|
|displayName|String|[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。|
|description|String|[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明|
|priority|Int32|優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。 ユーザーは、優先度の低い値を持つ構成のみに適用されます。 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承|
|createdDateTime|DateTimeOffset|[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時|
|lastModifiedDateTime|DateTimeOffset|[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。|
|version|Int32|[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン|
|pinMinimumLength|Int32|Windows Hello for Business の PIN に必要な最小文字数を制御します。  この値は、4 ~ 127 の範囲で、最大 PIN の値よりも小さいか等しい必要があります。|
|pinMaximumLength|Int32|Windows Hello for Business の PIN に使用できる最大文字数を制御します。 この値は、4 ~ 127 の範囲にする必要があります。 この値は、最小 PIN の値より大きいか等しい必要があります。|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Windows Hello for Business の PIN で大文字を使用する機能を制御します。  [許可] 大文字/小文字の使用が許可されますが、必要であれば必ず存在することを確認します。 [許可しない] に設定した場合、大文字は使用できません。 可能な値は、`allowed`、`required`、`disallowed` です。|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Windows Hello for Business の PIN で小文字を使用する機能を制御します。  許可されている場合は小文字の使用が許可されますが、必要であれば必ず存在することを確認してください。 [許可しない] に設定した場合、小文字は使用できません。 可能な値は、`allowed`、`required`、`disallowed` です。|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Windows Hello for Business の PIN で特殊文字を使用する機能を制御します。  許可されている場合、特殊文字の使用が許可されますが、必要に応じて存在することが保証されます。 [許可しない] に設定した場合、特殊文字は使用できません。 可能な値は、`allowed`、`required`、`disallowed` です。|
|state|[購入](../resources/intune-shared-enablement.md)|Windows Hello for Business 用にデバイスを構成することを許可するかどうかを制御します。 [無効] に設定されている場合、ユーザーは、必要に応じて、Azure Active Directory に参加しているモバイル電話を除き、Windows Hello for Business をプロビジョニングすることはできません。 未構成に設定した場合、Intune はクライアントの既定値を上書きしません。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|securityDeviceRequired|Boolean|Windows Hello for Business のプロビジョニングにトラステッドプラットフォームモジュール (TPM) を必要とするかどうかを制御します。 TPM に格納されたデータは、他のデバイスでは使用できないため、追加のセキュリティ上の利点があります。 False に設定されている場合は、使用可能な TPM がない場合でも、すべてのデバイスが Windows Hello for Business をプロビジョニングできます。|
|unlockWithBiometricsEnabled|Boolean|Windows Hello for Business PIN の代わりに、顔文字や指紋などのバイオメトリクスジェスチャの使用を制御します。  False に設定すると、生体認証ジェスチャは許可されません。 ユーザーは、障害が発生した場合に、バックアップとして PIN を構成する必要があります。|
|remotePassportEnabled|ブール型 (Boolean)|リモートの Windows Hello for Business の使用を制御します。 リモート Windows Hello for Business は、デスクトップ認証のコンパニオンとして使用できる、ポータブルで登録されたデバイスの機能を提供します。 デスクトップは Azure AD に参加している必要があります。コンパニオンデバイスには、Windows Hello for Business の PIN が必要です。|
|pinPreviousBlockCount|Int32|ユーザーが過去の Pin を使用できないようにする機能を制御します。 0 ~ 50 の範囲で設定する必要があり、ユーザーの現在の PIN がその数に含まれています。 0に設定すると、以前の Pin は保存されません。 Pin をリセットすると、PIN 履歴は保持されません。|
|pinExpirationInDays|Int32|ユーザーがシステムに PIN を変更することを要求するまでの時間 (日数) を制御します。 0 ~ 730 の範囲で設定する必要があります。 0に設定すると、ユーザーの PIN は期限切れになりません。|
|enhancedBiometricsState|[購入](../resources/intune-shared-enablement.md)|この機能をサポートするデバイス上の顔認識に対して、スプーフィング対策機能を使用する機能を制御します。 Disabled に設定した場合、スプーフィング対策機能は許可されません。 [未構成] に設定した場合、ユーザーはスプーフィング対策を使用するかどうかを選択できます。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|securityKeyForSignIn|[購入](../resources/intune-shared-enablement.md)|サインインのセキュリティキーでは、リモートでの Windows Hello Sercurity オン/オフの機能が提供されます。構成されていない構成は、clinet で行われる構成を優先します。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 667

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 839

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```






