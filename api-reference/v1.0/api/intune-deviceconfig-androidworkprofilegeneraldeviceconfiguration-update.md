---
title: androidwork profile、devic/デバイスの更新
description: androidwork profile、devic/オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1270136d1fa3d646dc96a60e93906c2ed37f248
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254010"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a>androidwork profile、devic/デバイスの更新

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[androidwork profile、devic/](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトのプロパティを更新します。

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
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [androidwork profileの devic/devicオブジェクト](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)の JSON 表記を指定します。

次の表に、 [androidwork profile[devic]](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|passwordBlockFingerprintUnlock|Boolean|指紋によるロック解除を禁止するかどうかを示します。|
|passwordBlockTrustAgents|Boolean|Smart Lock や他の信頼エージェントをブロックするかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限が切れるまでの日数。 有効な値は 1 から 365 までです|
|passwordMinimumLength|Int32|パスワードの最小の長さ。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordPreviousPasswordBlockCount|Int32|ブロックする、以前のパスワードの数。 有効な値は 0 から 24 までです|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。 有効な値は1から16までです|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|許可されているデータ共有の種類。 使用可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。|
|workProfileBlockNotificationsWhileDeviceLocked|Boolean|デバイスがロックされているときに通知をブロックするかどうかを示します。|
|ワークワークプロファイルのアカウント|Boolean|ユーザーが作業プロファイルでアカウントを追加または削除することを禁止します。|
|workProfileBluetoothEnableContactSharing|Boolean|bluetooth デバイスがエンタープライズの連絡先にアクセスできるようにします。|
|workProfileBlockScreenCapture|Boolean|作業プロファイルの画面キャプチャをブロックします。|
|work profileblockクロスバープロファイル ecallerid|Boolean|[ブロック表示作業プロファイルの発信者番号を個人プロファイルに表示する。|
|workProfileBlockCamera|Boolean|作業プロファイルカメラをブロックします。|
|workProfileBlockCrossProfileContactsSearch|Boolean|個人用プロファイルでの作業プロファイルの連絡先の使用を禁止します。|
|workProfileBlockCrossProfileCopyPaste|Boolean|[クロスプロファイルコピー/貼り付けを許可する] の設定が有効になっているかどうかを示すブール値。|
|work profiledefaultapppermissionpolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|必要なパスワードの種類。 使用可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。|
|。 workprofilepasswordblockfingerprintunlock|Boolean|ワークプロファイルの指紋のロック解除をブロックするかどうかを示します。|
|workProfilePasswordBlockTrustAgents|Boolean|ワークプロファイルのスマートロックおよびその他の信頼エージェントを禁止するかどうかを示します。|
|workProfilePasswordExpirationDays|Int32|作業プロファイルのパスワードが期限切れになるまでの日数。 有効な値は 1 から 365 までです|
|workProfilePasswordMinimumLength|Int32|ワークプロファイルのパスワードの最小の長さ。 有効な値は 4 から 16 までです|
|ワークプロファイルのパスワード minnumericcharacters|Int32|作業プロファイルのパスワードに必要な数字の最小数。 有効な値は1から10までです|
|workProfilePasswordMinNonLetterCharacters|Int32|作業プロファイルのパスワードに必要な文字以外の文字数の最小値。 有効な値は1から10までです|
|workProfilePasswordMinLetterCharacters|Int32|作業プロファイルのパスワードに必要な文字数の最小値。 有効な値は1から10までです|
|workProfilePasswordMinLowerCaseCharacters|Int32|作業プロファイルのパスワードに必要な小文字の最小文字数。 有効な値は1から10までです|
|workProfilePasswordMinUpperCaseCharacters|Int32|作業プロファイルのパスワードに必要な大文字と小文字の最小値。 有効な値は1から10までです|
|ワークスペースのパスワードを入力する|Int32|作業プロファイルのパスワードに必要な記号の最小数。 有効な値は1から10までです|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|workProfilePasswordPreviousPasswordBlockCount|Int32|ブロックする、以前の作業プロファイルのパスワードの数。 有効な値は 0 から 24 までです|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|作業プロファイルが削除され、すべての企業データが削除されるまでに許可されるサインイン失敗回数。 有効な値は1から16までです|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|必要な業務プロファイルのパスワードの種類。 可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。|
|次|Boolean|パスワードが必要です。または職場プロファイルでは使用できません|
|securityRequireVerifyApps|Boolean|Android の検証アプリ機能をオンにするよう要求します。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidwork profileprofiledevicオブジェクト](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)を返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```



