---
title: depIOSEnrollmentProfile リソースの種類
description: DepIOSEnrollmentProfile リソースは、iOS 構成固有の Apple Device Enrollment Program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが DEP を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 739d8bc495cebbc00837b325f68002a5ee8e9903
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328040"
---
# <a name="depiosenrollmentprofile-resource-type"></a>depIOSEnrollmentProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DepIOSEnrollmentProfile リソースは、iOS 構成固有の Apple Device Enrollment Program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが DEP を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。


[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)コレクション|[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DepIOSEnrollmentProfile を取得する](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DepIOSEnrollmentProfile を作成する](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|新しい[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを作成します。|
|[DepIOSEnrollmentProfile の削除](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|None|[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)を削除します。|
|[DepIOSEnrollmentProfile の更新](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|[DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID|
|displayName|String|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前|
|description|String|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明|
|requiresUserAuthentication|Boolean|プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。|
|configurationEndpointUrl|String|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url|
|enableAuthenticationViaCompanyPortal|Boolean|会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。 [しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。|
|isDefault|ブール型 (Boolean)|これが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された既定のプロファイルであるかどうかを示します。|
|supervisedModeEnabled|Boolean|監視モード、有効にする場合は True、それ以外の場合は false。 詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。 [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。|
|supportDepartment|String|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート部署情報|
|Pass Codedisabled|Boolean|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたパスコードセットアップウィンドウが無効であるかどうかを示します|
|isMandatory|Boolean|プロファイルが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。|
|locationDisabled|Boolean|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された場所サービスのセットアップウィンドウが無効になっているかどうかを示します。|
|supportPhoneNumber|String|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたサポート電話番号|
|profileRemovalDisabled|Boolean|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたプロファイル削除オプションが無効になっているかどうかを示します。|
|restoreBlocked|Boolean|復元のセットアップウィンドウが[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されているかどうかを示します。|
|りんご Eiddisabled|Boolean|Apple id のセットアップウィンドウが無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。|
|termsAndConditionsDisabled|Boolean|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された [使用条件] 設定ウィンドウを無効にするかどうかを示します。|
|touchIdDisabled|Boolean|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたタッチ id セットアップウィンドウを無効にするかどうかを示します|
|applePayDisabled|Boolean|Apple の [支払い設定] ウィンドウが無効にされているかどうかを[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。|
|zoomDisabled|Boolean|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承されたズーム設定ウィンドウが無効であるかどうかを示します|
|siriDisabled|Boolean|Siri セットアップウィンドウが無効であるかどうかを示します ( [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承)|
|diagnosticsDisabled|Boolean|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承された診断セットアップウィンドウが無効であるかどうかを示します|
|displayToneSetupDisabled|Boolean|Displaytone セットアップ画面が無効になっているかどうかを示します[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。|
|privacyPaneDisabled|Boolean|プライバシー画面が無効にされているかどうかを示します。 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。|
|deviceNameTemplate|String|リテラルまたは名前のパターンを設定します。 [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|ITunes ペアリングモードを示します。 可能な値は、`disallow`、`allow`、`requiresCertificate` です。|
|managementCertificates|[Managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション|Apple Configurator の管理証明書|
|restoreFromAndroidDisabled|Boolean|Android からの復元が無効であるかどうかを示します|
|awaitDeviceConfiguredConfirmation|Boolean|構成済みの確認をデバイスが待機する必要があるかどうかを示します|
|sharedIPadMaximumUserCount|Int32|これにより、共有 iPad を使用できるユーザーの最大数が指定されます。 共有 iPad モードでのみ適用されます。|
|enableSharedIPad|Boolean|これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。 共有 Ipad にのみ適用されます。|
|companyPortalVppTokenId|String|設定されている場合は、ポータルサイトのライセンスを展開するためにどの Vpp トークンを使用する必要があるかを示します。 このプロパティを設定するためには、' enableAuthenticationViaCompanyPortal ' を設定する必要があります。|
|enableSingleAppEnrollmentMode|Boolean|デバイスに対して、1つのアプリモードを有効にし、登録時にアプリロックを適用するように指示します。 既定値は false です。 このプロパティを設定するには、' enableAuthenticationViaCompanyPortal ' および ' companyPortalVppTokenId ' を設定する必要があります。|
|ホームボタンの無効化|Boolean|[ホームボタンの感度] 画面を無効にするかどうかを示します|
|iMessageAndFaceTimeScreenDisabled|Boolean|IMessage および FaceTime の画面が無効であるかどうかを示します|
|onBoardingScreenDisabled|Boolean|オンボードのセットアップ画面が無効であるかどうかを示します|
|screenTimeScreenDisabled|Boolean|画面のタイムアウト設定を無効にするかどうかを示します。|
|シムの設定を無効にする|Boolean|[シム] セットアップ画面が無効であるかどうかを示します。|
|ソフトウェアの更新 Creendisabled|Boolean|必須の [ソフトウェアの更新] 画面が無効であるかどうかを示します。|
|watchMigrationScreenDisabled|Boolean|[移行の監視] 画面が無効であるかどうかを示します|

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
  "deviceNameTemplate": "String",
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



