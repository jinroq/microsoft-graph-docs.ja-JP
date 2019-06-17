---
title: depEnrollmentBaseProfile リソースの種類
description: DepEnrollmentBaseProfile リソースは、Apple Device Enrollment Program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが DEP を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b92a86a3faa3da1af203e3688b7de7318a76dca4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978914"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>depEnrollmentBaseProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DepEnrollmentBaseProfile リソースは、Apple Device Enrollment Program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが DEP を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。


[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)コレクション|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DepEnrollmentBaseProfile を取得する](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|

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
|isDefault|ブール型 (Boolean)|これが既定のプロファイルであるかどうかを示します|
|supervisedModeEnabled|Boolean|監視モード、有効にする場合は True、それ以外の場合は false。 詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。|
|supportDepartment|String|サポート部門の情報|
|Pass Codedisabled|Boolean|パスコードセットアップウィンドウが無効であるかどうかを示します|
|isMandatory|Boolean|プロファイルが必須であるかどうかを示します|
|locationDisabled|Boolean|場所サービスの設定ウィンドウが無効であるかどうかを示します|
|supportPhoneNumber|String|サポート電話番号|
|profileRemovalDisabled|Boolean|プロファイルの削除オプションが無効になっているかどうかを示します|
|restoreBlocked|Boolean|セットアップウィンドウの復元がブロックされているかどうかを示します|
|りんご Eiddisabled|Boolean|Apple id のセットアップウィンドウが無効であるかどうかを示します|
|termsAndConditionsDisabled|Boolean|[使用条件] セットアップウィンドウが無効かどうかを示します|
|touchIdDisabled|Boolean|タッチ id のセットアップウィンドウが無効であるかどうかを示します|
|applePayDisabled|Boolean|Apple の支払い設定ウィンドウが無効であるかどうかを示します|
|zoomDisabled|Boolean|ズーム設定ウィンドウが無効であるかどうかを示します|
|siriDisabled|Boolean|Siri セットアップウィンドウが無効であるかどうかを示します|
|diagnosticsDisabled|Boolean|診断セットアップウィンドウが無効であるかどうかを示します|
|displayToneSetupDisabled|Boolean|Displaytone の設定画面が無効であるかどうかを示します|
|privacyPaneDisabled|Boolean|プライバシー画面が無効であるかどうかを示します|
|deviceNameTemplate|String|リテラルまたは名前のパターンを設定します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
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
  "deviceNameTemplate": "String"
}
```





