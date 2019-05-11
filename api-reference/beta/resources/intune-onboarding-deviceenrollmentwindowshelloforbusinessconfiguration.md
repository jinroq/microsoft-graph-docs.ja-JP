---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration リソースの種類
description: Windows Hello for Business の設定を使用すると、ユーザーは、バイオメトリクス認証などのジェスチャを使用してデバイスにアクセスできます。または、PIN を使用します。 登録済みの Windows 10、Windows 10 Mobile 以降の設定を構成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f98f590f049f1941ddcc0a721d66e27b6c56f373
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940408"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>deviceEnrollmentWindowsHelloForBusinessConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows Hello for Business の設定を使用すると、ユーザーは、バイオメトリクス認証などのジェスチャを使用してデバイスにアクセスできます。または、PIN を使用します。 登録済みの Windows 10、Windows 10 Mobile 以降の設定を構成します。


[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceEnrollmentWindowsHelloForBusinessConfigurations](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-list.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) コレクション|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。|
|[Delete deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-delete.md)|なし|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) を削除します。|
|[Update deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
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

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション|[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス構成プロファイルのグループ割り当ての一覧|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "state": "String",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 1024,
  "pinExpirationInDays": 1024,
  "enhancedBiometricsState": "String"
}
```




