---
title: depEnrollmentBaseProfile リソースの種類
description: DepEnrollmentBaseProfile リソースは、Apple Device enrollment program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが dep を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5ad27470bb09313084feadcf468d83e58964532
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143107"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>depEnrollmentBaseProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DepEnrollmentBaseProfile リソースは、Apple Device enrollment program (DEP) 登録プロファイルを表します。 この種類のプロファイルは、対応するデバイスが dep を使用して登録できるようになる前に、Apple DEP シリアル番号に割り当てる必要があります。


[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)コレクション|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[depEnrollmentBaseProfile を取得する](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたオブジェクトの GUID|
|displayName|String|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの名前|
|説明|String|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたプロファイルの説明|
|requiresUserAuthentication|ブール値|プロファイルが[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承したユーザー認証を必要とするかどうかを示します。|
|configurationendpointurl|String|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承された登録に使用する構成エンドポイント url|
|enableAuthenticationViaCompanyPortal|ブール値|会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。 [しました](../resources/intune-enrollment-enrollmentprofile.md)から継承します。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|ブール値|[しました](../resources/intune-enrollment-enrollmentprofile.md)から継承されたセットアップアシスタントの登録済みデバイスで、会社のポータルが必要であることを示します。|
|isDefault|ブール値|これが既定のプロファイルであるかどうかを示します|
|supervisedModeEnabled|ブール値|監視モード、有効にする場合は True、それ以外の場合は false。 詳細https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intuneについては、「」を参照してください。|
|supportdepartment|String|サポート部門の情報|
|pass codedisabled|ブール値|パスコードセットアップウィンドウが無効であるかどうかを示します|
|ismandatory|ブール値|プロファイルが必須であるかどうかを示します|
|locationdisabled|ブール値|場所サービスの設定ウィンドウが無効であるかどうかを示します|
|supportPhoneNumber|String|サポート電話番号|
|profileRemovalDisabled|ブール値|プロファイルの削除オプションが無効になっているかどうかを示します|
|restoreblocked|ブール値|セットアップウィンドウの復元がブロックされているかどうかを示します|
|りんご eiddisabled|ブール値|Apple id のセットアップウィンドウが無効であるかどうかを示します|
|termsAndConditionsDisabled|ブール値|[使用条件] セットアップウィンドウが無効かどうかを示します|
|touchIdDisabled|ブール値|タッチ id のセットアップウィンドウが無効であるかどうかを示します|
|applePayDisabled|ブール値|Apple の支払い設定ウィンドウが無効であるかどうかを示します|
|zoomDisabled|ブール値|ズーム設定ウィンドウが無効であるかどうかを示します|
|siridisabled|ブール値|siri セットアップウィンドウが無効であるかどうかを示します|
|diagnosticsDisabled|ブール値|診断セットアップウィンドウが無効であるかどうかを示します|
|displayToneSetupDisabled|ブール値|displaytone の設定画面が無効であるかどうかを示します|
|privacyPaneDisabled|ブール値|プライバシー画面が無効であるかどうかを示します|

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
  "privacyPaneDisabled": true
}
```




