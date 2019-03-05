---
title: windowsIdentityProtectionConfiguration の更新
description: windowsIdentityProtectionConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14b8a94c8a27ec06187b342af5619433c48ccce9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141294"
---
# <a name="update-windowsidentityprotectionconfiguration"></a>windowsIdentityProtectionConfiguration の更新

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトの JSON 表記を指定します。

次の表に、 [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)の作成時に必要なプロパティを示します。

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
|useSecurityKeyForSignin|Boolean|ログオン資格情報として Windows Hello セキュリティキーを有効にするために使用されるブール値。|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boolean|Windows Hello 顔認証で顔機能認識の強化されたスプーフィング対策を有効にするために使用するブール値。|
|pinMinimumLength|Int32|Windows Hello for business の PIN に必要な最小文字数を設定する整数値。 有効な値は、4 ~ 127 の範囲で、最大 PIN の値を設定します。 有効な値は 4 ~ 127|
|pinMaximumLength|Int32|作業 PIN に使用できる最大文字数を設定する整数値。 有効な値は、最小 PIN で設定された値以上の4から127の範囲です。 有効な値は 4 ~ 127|
|pinUppercaseCharactersUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|この値は、Windows Hello for Business の PIN での大文字の使用を構成します。 可能な値は `blocked`、`required`、`allowed` です。|
|pinLowercaseCharactersUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|この値は、Windows Hello for Business の PIN に小文字を使用するように構成します。 可能な値は `blocked`、`required`、`allowed` です。|
|pinSpecialCharactersUsage|[configurationusage](../resources/intune-deviceconfig-configurationusage.md)|Windows Hello for Business の PIN で特殊文字を使用する機能を制御します。 可能な値は `blocked`、`required`、`allowed` です。|
|pinExpirationInDays|Int32|[整数値] PIN の変更をユーザーに要求する前に PIN を使用できる期間 (日数) を指定します。 有効な値は0から730の範囲です。 有効な値は 0 から 730 までです|
|pinPreviousBlockCount|Int32|ユーザーが過去の pin を使用できないようにする機能を制御します。 0 ~ 50 の範囲で設定する必要があり、ユーザーの現在の PIN がその数に含まれています。 0に設定すると、以前の pin は保存されません。 pin をリセットすると、pin 履歴は保持されません。 有効な値は 0 から 50 までです|
|pinrecoveryenabled|Boolean|ユーザーが Windows Hello for business pin 回復サービスを使用して pin を変更できるようにするブール値。|
|securityDeviceRequired|Boolean|Windows Hello for business のプロビジョニングにトラステッドプラットフォームモジュール (TPM) を必要とするかどうかを制御します。 TPM に格納されたデータは、他のデバイスでは使用できないため、追加のセキュリティ上の利点があります。 False に設定されている場合は、使用可能な TPM がない場合でも、すべてのデバイスが Windows Hello for business をプロビジョニングできます。|
|unlockWithBiometricsEnabled|Boolean|Windows Hello for Business PIN の代わりに、顔文字や指紋などのバイオメトリクスジェスチャの使用を制御します。  False に設定すると、生体認証ジェスチャは許可されません。 ユーザーは、障害が発生した場合に、バックアップとして PIN を構成する必要があります。|
|useCertificatesForOnPremisesAuthEnabled|Boolean|Windows Hello for business が証明書を使用してオンプレミスのリソースを認証できるようにするブール値。|
|windowsHelloForBusinessBlocked|Boolean|windows Hello for business を windows にサインインするための方法としてブロックするブール値。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 982

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```




