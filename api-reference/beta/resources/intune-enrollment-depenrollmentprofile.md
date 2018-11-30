---
title: depEnrollmentProfile リソースの種類
description: DepEnrollmentProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。 このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。
ms.openlocfilehash: 5c09bac440d2dce8cb141787d0809c74aed747c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073886"
---
# <a name="depenrollmentprofile-resource-type"></a>depEnrollmentProfile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

DepEnrollmentProfile リソースでは、アップル デバイスの登録プログラム (DEP) の登録プロファイルを表します。 このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。

[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)コレクション|[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティと関係を一覧表示します。|
|[DepEnrollmentProfile を取得します。](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[DepEnrollmentProfile を作成します。](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|新しい[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトを作成します。|
|[DepEnrollmentProfile を削除します。](../api/intune-enrollment-depenrollmentprofile-delete.md)|なし|の[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)を削除します。|
|[DepEnrollmentProfile を更新します。](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID|
|displayName|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前|
|説明|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明|
|requiresUserAuthentication|ブール値|プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します|
|configurationEndpointUrl|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成|
|enableAuthenticationViaCompanyPortal|ブール値|アップルらくらく企業ポータルではなくを使用して認証することを示します。 [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。|
|isDefault|ブール値|これは、既定のプロファイルであるかどうかを示します|
|supervisedModeEnabled|ブール値|コールを管理モードを有効にする、false それ以外の場合は True です。 参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。|
|supportDepartment|String|サポート部門の情報|
|passCodeDisabled|ブール値|パスコードの設定] ウィンドウが無効になっているかどうかを示します|
|isMandatory|ブール値|プロファイルが必須かどうかを|
|locationDisabled|ブール値|場所サービス セットアップ] ウィンドウが無効になっているかどうかを示します|
|supportPhoneNumber|String|サポート電話番号|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|ITunes のペアリング モードを示します。 可能な値は、`disallow`、`allow`、`requiresCertificate` です。|
|profileRemovalDisabled|ブール値|プロファイルの削除オプションが無効になっているかどうかを示します|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション|Apple Configurator の証明書を管理|
|restoreBlocked|ブール値|復元の設定] ウィンドウがブロックされていることを示します。|
|restoreFromAndroidDisabled|ブール値|Android からの復元が無効になっているかどうかを示します|
|appleIdDisabled|ブール値|Apple id の設定] ウィンドウが無効になっているかどうかを示します|
|termsAndConditionsDisabled|ブール値|'条項および条件' の設定ウィンドウが無効になっているかどうかを示します|
|touchIdDisabled|ブール値|タッチ id の設定] ウィンドウが無効になっているかどうかを示します|
|applePayDisabled|ブール値|アップル支払設定] ウィンドウが無効になっているかどうかを示します|
|zoomDisabled|ブール値|ズームの設定] ウィンドウが無効になっているかどうかを示します|
|siriDisabled|ブール値|Siri の設定] ウィンドウが無効になっているかどうかを示します|
|diagnosticsDisabled|ブール値|診断設定] ウィンドウが無効になっているかどうかを示します|
|macOSRegistrationDisabled|ブール値|Mac OS の登録が無効になっているかどうかを示します|
|macOSFileVaultDisabled|ブール値|Mac OS ファイルのボルトが無効になっているかどうかを示します|
|awaitDeviceConfiguredConfirmation|ブール値|デバイスが構成されている確認メッセージを待機する必要がかどうかを示します|
|sharedIPadMaximumUserCount|Int32|共有の iPad を使用できるユーザーの最大数を指定します。 IPad を共有モードでのみ適用できます。|
|enableSharedIPad|ブール値|これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。 共有台もの Ipad でのみ適用できます。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
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
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```





