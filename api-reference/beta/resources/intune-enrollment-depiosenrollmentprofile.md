---
title: depIOSEnrollmentProfile リソースの種類
description: DepIOSEnrollmentProfile リソースでは、iOS の構成を特定の Apple デバイスの登録プログラム (DEP) 登録プロファイルを表します。 このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0068921c65085417712efbe41e9145ac0b122cab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400894"
---
# <a name="depiosenrollmentprofile-resource-type"></a>depIOSEnrollmentProfile リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DepIOSEnrollmentProfile リソースでは、iOS の構成を特定の Apple デバイスの登録プログラム (DEP) 登録プロファイルを表します。 このタイプのプロファイルは、DEP. を使用して対応するデバイスを登録する前に、Apple の DEP のシリアル番号を割り当てる必要があります。


[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)コレクション|[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティと関係を一覧表示します。|
|[DepIOSEnrollmentProfile を取得します。](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[DepIOSEnrollmentProfile を作成します。](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|新しい[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを作成します。|
|[DepIOSEnrollmentProfile を削除します。](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|なし|の[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)を削除します。|
|[DepIOSEnrollmentProfile を更新します。](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるオブジェクトの GUID|
|displayName|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの名前|
|説明|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるプロファイルの説明|
|requiresUserAuthentication|Boolean|プロファイルに[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されるのユーザー認証が必要なかどうかを示します|
|configurationEndpointUrl|String|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から登録の継承を使用するエンドポイントの url を構成|
|enableAuthenticationViaCompanyPortal|Boolean|アップルらくらく企業ポータルではなくを使用して認証することを示します。 [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)から継承されました。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|継承セットアップ アシスタントが登録されているデバイスは、 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)からの会社のポータルが必要であることを示します。|
|isDefault|Boolean|これは、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承される既定のプロファイルであるかどうかを示します|
|supervisedModeEnabled|Boolean|コールを管理モードを有効にする、false それ以外の場合は True です。 参照してくださいhttps://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneの追加情報です。 [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|supportDepartment|String|継承のサポート部門については、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から|
|passCodeDisabled|Boolean|パスコードの設定] ウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します|
|isMandatory|Boolean|プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承が必須であるかを示す|
|locationDisabled|Boolean|サービス セットアップ] ウィンドウの場所が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します|
|supportPhoneNumber|String|継承のサポート電話番号は、 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から|
|profileRemovalDisabled|Boolean|プロファイルの削除オプションが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|restoreBlocked|Boolean|復元の設定] ウィンドウがブロックされていることを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|appleIdDisabled|Boolean|Id の設定] ウィンドウは、Apple が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します|
|termsAndConditionsDisabled|Boolean|'条項および条件' の設定ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|touchIdDisabled|Boolean|タッチ id の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|applePayDisabled|Boolean|アップル支払設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|zoomDisabled|Boolean|ズームの設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|siriDisabled|Boolean|Siri の設定] ウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|diagnosticsDisabled|Boolean|設定] ウィンドウは、診断が[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)からの継承を無効になってかどうかを示します|
|displayToneSetupDisabled|Boolean|Displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|privacyPaneDisabled|Boolean|プライバシー画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されました。|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|ITunes のペアリング モードを示します。 可能な値は、`disallow`、`allow`、`requiresCertificate` です。|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション|Apple Configurator の証明書を管理|
|restoreFromAndroidDisabled|Boolean|Android からの復元が無効になっているかどうかを示します|
|awaitDeviceConfiguredConfirmation|Boolean|デバイスが構成されている確認メッセージを待機する必要がかどうかを示します|
|sharedIPadMaximumUserCount|Int32|共有の iPad を使用できるユーザーの最大数を指定します。 IPad を共有モードでのみ適用できます。|
|enableSharedIPad|Boolean|これは、デバイスが、マルチ ユーザー シナリオを有効にするモードに登録するかどうかを示します。 共有台もの Ipad でのみ適用できます。|
|companyPortalVppTokenId|String|場合設定、デバイスのライセンスと企業ポータルを展開するどの Vpp トークンを使用する必要があることを示します。 'enableAuthenticationViaCompanyPortal' は、このプロパティを設定するために設定する必要があります。|
|enableSingleAppEnrollmentMode|Boolean|1 つのアプリケーション モードを有効にして、登録時にアプリケーション ロックを適用するデバイスを指示します。 既定では false を指定します。 'enableAuthenticationViaCompanyPortal' と 'companyPortalVppTokenId' は、このプロパティを設定するのに設定してください。|
|homeButtonScreenDisabled|Boolean|感度画面の [ホーム] ボタンが無効になっているかどうかを示します|
|iMessageAndFaceTimeScreenDisabled|Boolean|場合 iMessage、FaceTime の画面が無効になります|
|onBoardingScreenDisabled|Boolean|契約時のセットアップ画面が無効になっているかどうかを示します|
|screenTimeScreenDisabled|Boolean|画面のタイムアウトの設定が無効になっているかどうかを示します|
|simSetupScreenDisabled|Boolean|SIMSetup 画面が無効になっているかどうかを示します|
|softwareUpdateScreenDisabled|Boolean|必須のソフトウェアの更新] 画面が無効になっているかどうかを示します|
|watchMigrationScreenDisabled|Boolean|ウォッチ移行] 画面が無効になっているかどうかを示します|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




