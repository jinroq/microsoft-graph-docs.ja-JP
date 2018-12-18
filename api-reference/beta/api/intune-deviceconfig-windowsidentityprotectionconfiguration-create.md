---
title: WindowsIdentityProtectionConfiguration を作成します。
description: 新しい windowsIdentityProtectionConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: a0d588943f75694af159cfd835fc2e3a09b052e0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355392"
---
# <a name="create-windowsidentityprotectionconfiguration"></a>WindowsIdentityProtectionConfiguration を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを作成します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

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
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に windowsIdentityProtectionConfiguration オブジェクトの JSON の形式を指定します。

次の表は、windowsIdentityProtectionConfiguration を作成するときに必要なプロパティを示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール型|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|enhancedAntiSpoofingForFacialFeaturesEnabled|ブール型|拡張スプーフィング対策 Windows こんにちは顔認証の facial の機能の認識を有効にするために使用するブール値です。|
|pinMinimumLength|Int32|ビジネスの暗証番号 (pin) は、Windows こんにちはに必要な文字の最小数を設定する整数値。 有効な値は 4 ~ 127 包括的で、最大の暗証番号 (pin) の設定値に等しいかそれより小さい。 有効な値 4 ~ 127|
|pinMaximumLength|Int32|暗証番号 (pin) の作業に使用できる文字の最大数を設定する整数値。 有効な値は、4 ~ 127 包括的以上の最小の暗証番号 (pin) の設定値と同じです。 有効な値 4 ~ 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|この値は、ビジネスの暗証番号 (pin) の Windows こんにちはの文字の大文字の使用を構成します。 可能な値は、`blocked`、`required`、`allowed` です。|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|この値は、ビジネスの暗証番号 (pin) の Windows こんにちはで小文字の使用を構成します。 可能な値は、`blocked`、`required`、`allowed` です。|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|ビジネスの暗証番号 (pin) を Windows こんにちはで特殊文字を使用する機能を制御します。 可能な値は、`blocked`、`required`、`allowed` です。|
|pinExpirationInDays|Int32|期間 (日数) を指定する整数値システムがそれを変更するユーザーを必要とする前に、暗証番号 (pin) を使用することができます。 有効な値は、0 に 730 包括的です。 有効な値は 0 から 730 までです|
|pinPreviousBlockCount|Int32|過去のピンを使用できないようにする機能を制御します。 0 から 50、包括的で、これを設定する必要があり、その数にユーザーの現在の暗証番号 (pin) が含まれています。 かどうかは 0 では、以前に設定ピンは格納されません。 PIN を通じて暗証番号 (pin) の履歴は保持されませんをリセットします。 有効な値は 0 から 50 までです|
|pinRecoveryEnabled|ブール型|使用して、Windows こんにちはビジネス暗証番号 (pin) リカバリ ・ サービスの PIN を変更するユーザーを有効にするブール値です。|
|securityDeviceRequired|Boolean|Windows こんにちはビジネスのための準備のトラステッド プラットフォーム モジュール (TPM) を必要とするかどうかを制御します。 TPM は、他のデバイス上に格納されているデータは使用できませんという点で、その他セキュリティ上の利点を提供します。 かどうかは False に設定すると、すべてのデバイスをプロビジョニングできる Windows こんにちはビジネスに使用可能な TPM がない場合でも。|
|unlockWithBiometricsEnabled|Boolean|代わりに、Windows こんにちはビジネス暗証番号 (pin) の顔や指紋などの生体認証のジェスチャの使用を制御します。  場合は False、生体認証のジェスチャに設定することはできません。 ユーザーは、障害が発生した場合のバックアップとして、暗証番号 (pin) を構成する必要があります。|
|useCertificatesForOnPremisesAuthEnabled|ブール型|Windows こんにちは設置型リソースの認証に証明書を使用するビジネスを可能にするブール値です。|
|windowsHelloForBusinessBlocked|Boolean|Windows こんにちはの Windows へのサインイン方法としてビジネスをブロックするブール値です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 838

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 946

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





