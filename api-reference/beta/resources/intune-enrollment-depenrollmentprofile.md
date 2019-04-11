---
title: depEnrollmentProfile リソースの種類
description: depEnrollmentProfile リソースは、Apple Device enrollment program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが dep を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4a365ee8a83820789ecdbf199df5997b6e683e0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806098"
---
# <a name="depenrollmentprofile-resource-type"></a>depEnrollmentProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

depEnrollmentProfile リソースは、Apple Device enrollment program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが dep を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。


[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)コレクション|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[depEnrollmentProfile を取得する](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[depEnrollmentProfile を作成する](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|新しい[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトを作成します。|
|[depEnrollmentProfile の削除](../api/intune-enrollment-depenrollmentprofile-delete.md)|なし|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)を削除します。|
|[depEnrollmentProfile の更新](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID|
|displayName|String|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前|
|説明|String|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明|
|requiresUserAuthentication|Boolean|プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。|
|configurationendpointurl|文字列|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url|
|enableAuthenticationViaCompanyPortal|Boolean|会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。 [しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。|
|isDefault|ブール型 (Boolean)|これが既定のプロファイルであるかどうかを示します|
|supervisedModeEnabled|Boolean|監視モード、有効にする場合は True、それ以外の場合は false。 詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。|
|supportdepartment|文字列|サポート部門の情報|
|pass codedisabled|Boolean|パスコードセットアップウィンドウが無効であるかどうかを示します|
|ismandatory|Boolean|プロファイルが必須であるかどうかを示します|
|locationdisabled|Boolean|場所サービスの設定ウィンドウが無効であるかどうかを示します|
|supportPhoneNumber|文字列|サポート電話番号|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|iTunes ペアリングモードを示します。 使用可能な値は、`disallow`、`allow`、`requiresCertificate` です。|
|profileRemovalDisabled|Boolean|プロファイルの削除オプションが無効になっているかどうかを示します|
|managementcertificates|[managementcertificatewiththumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)コレクション|Apple Configurator の管理証明書|
|restoreblocked|Boolean|セットアップウィンドウの復元がブロックされているかどうかを示します|
|restoreFromAndroidDisabled|Boolean|Android からの復元が無効であるかどうかを示します|
|りんご eiddisabled|Boolean|Apple id のセットアップウィンドウが無効であるかどうかを示します|
|termsAndConditionsDisabled|Boolean|[使用条件] セットアップウィンドウが無効かどうかを示します|
|touchIdDisabled|Boolean|タッチ id のセットアップウィンドウが無効であるかどうかを示します|
|applePayDisabled|Boolean|Apple の支払い設定ウィンドウが無効であるかどうかを示します|
|zoomDisabled|Boolean|ズーム設定ウィンドウが無効であるかどうかを示します|
|siridisabled|Boolean|siri セットアップウィンドウが無効であるかどうかを示します|
|diagnosticsDisabled|Boolean|診断セットアップウィンドウが無効であるかどうかを示します|
|macosregistrationdisabled|Boolean|Mac OS 登録が無効であるかどうかを示します|
|macOSFileVaultDisabled|Boolean|Mac OS ファイルボルトが無効であるかどうかを示します|
|awaitDeviceConfiguredConfirmation|Boolean|構成済みの確認をデバイスが待機する必要があるかどうかを示します|
|sharedIPadMaximumUserCount|Int32|これにより、共有 iPad を使用できるユーザーの最大数が指定されます。 共有 iPad モードでのみ適用されます。|
|enableSharedIPad|Boolean|これは、デバイスを、複数のユーザーシナリオを有効にするモードで登録するかどうかを示します。 共有 ipad にのみ適用されます。|

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
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
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





