---
title: DepEnrollmentProfile を更新します。
description: DepEnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a25f9604f0fd7808cb938dc1720e137db825ab4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983185"
---
# <a name="update-depenrollmentprofile"></a>DepEnrollmentProfile を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトの JSON の形式を指定します。

[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID|
|displayName|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前|
|説明|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明|
|requiresUserAuthentication|ブール型|プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します|
|configurationEndpointUrl|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成|
|enableAuthenticationViaCompanyPortal|ブール型|アップルらくらく企業ポータルではなくを使用して認証することを示します。 [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。|
|isDefault|ブール型|これは、既定のプロファイルであるかどうかを示します|
|supervisedModeEnabled|ブール型|コールを管理モードを有効にする、false それ以外の場合は True です。 参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。|
|supportDepartment|String|サポート部門の情報|
|passCodeDisabled|ブール型|パスコードの設定] ウィンドウが無効になっているかどうかを示します|
|isMandatory|ブール型|プロファイルが必須かどうかを|
|locationDisabled|ブール型|場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します|
|supportPhoneNumber|String|サポート電話番号|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|ITunes のペアリング モードを示します。 可能な値は、`disallow`、`allow`、`requiresCertificate` です。|
|profileRemovalDisabled|ブール型|プロファイルの削除オプションが無効になっているかどうかを示します|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション|Apple Configurator の証明書を管理|
|restoreBlocked|ブール型|復元の設定] ウィンドウがブロックされていることを示します。|
|restoreFromAndroidDisabled|ブール型|Android からの復元が無効になっているかどうかを示します|
|appleIdDisabled|ブール型|Apple id の設定] ウィンドウが無効になっているかどうかを示します|
|termsAndConditionsDisabled|ブール型|'条項および条件' の設定ウィンドウが無効になっているかどうかを示します|
|touchIdDisabled|ブール型|タッチ id の設定] ウィンドウが無効になっているかどうかを示します|
|applePayDisabled|ブール型|アップル支払設定] ウィンドウが無効になっているかどうかを示します|
|zoomDisabled|ブール型|ズームの設定] ウィンドウが無効になっているかどうかを示します|
|siriDisabled|ブール型|Siri の設定] ウィンドウが無効になっているかどうかを示します|
|diagnosticsDisabled|ブール型|診断設定] ウィンドウが無効になっているかどうかを示します|
|macOSRegistrationDisabled|ブール型|Mac OS の登録が無効になっているかどうかを示します|
|macOSFileVaultDisabled|ブール型|Mac OS ファイルのボルトが無効になっているかどうかを示します|
|awaitDeviceConfiguredConfirmation|ブール型|デバイスが構成されている確認メッセージを待機する必要がかどうかを示します|
|sharedIPadMaximumUserCount|Int32|共有の iPad を使用できるユーザーの最大数を指定します。 IPad を共有モードでのみ適用できます。|
|enableSharedIPad|ブール型|これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。 共有台もの Ipad でのみ適用できます。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1231

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1339

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```





