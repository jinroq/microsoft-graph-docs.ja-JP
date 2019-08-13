---
title: depMacOSEnrollmentProfile リソースの種類
description: DepMacOSEnrollmentProfile リソースは、macOS 構成に固有の Apple Device Enrollment Program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが DEP を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dec020828cd01fde2b3709d8290c5488e53b67c0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328047"
---
# <a name="depmacosenrollmentprofile-resource-type"></a>depMacOSEnrollmentProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DepMacOSEnrollmentProfile リソースは、macOS 構成に固有の Apple Device Enrollment Program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが DEP を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。


[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト depMacOSEnrollmentProfiles](../api/intune-enrollment-depmacosenrollmentprofile-list.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)コレクション|[DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DepMacOSEnrollmentProfile を取得する](../api/intune-enrollment-depmacosenrollmentprofile-get.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|[DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DepMacOSEnrollmentProfile を作成する](../api/intune-enrollment-depmacosenrollmentprofile-create.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|新しい[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトを作成します。|
|[DepMacOSEnrollmentProfile の削除](../api/intune-enrollment-depmacosenrollmentprofile-delete.md)|None|[DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)を削除します。|
|[DepMacOSEnrollmentProfile の更新](../api/intune-enrollment-depmacosenrollmentprofile-update.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|[DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトのプロパティを更新します。|

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
|registrationDisabled|Boolean|登録が無効であるかどうかを示します|
|fileVaultDisabled|Boolean|ファイルボルトが無効であるかどうかを示します|
|iCloudDiagnosticsDisabled|Boolean|ICloud 分析画面が無効かどうかを示します|
|iCloudStorageDisabled|Boolean|ICloud ドキュメントとデスクトップ画面が無効かどうかを示します|
|[Lockscreenを無効にする] を設定します。|Boolean|ICloud ドキュメントとデスクトップ画面が無効かどうかを示します|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depMacOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```



