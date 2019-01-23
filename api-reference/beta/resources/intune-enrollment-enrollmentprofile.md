---
title: enrollmentProfile リソースの種類
description: EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。 ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a7ce4aac1e22610d539419dd6a63d124616b83f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396841"
---
# <a name="enrollmentprofile-resource-type"></a>enrollmentProfile リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。 ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)コレクション|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティと関係を一覧表示します。|
|[EnrollmentProfile を取得します。](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[EnrollmentProfile を作成します。](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|新しい[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。|
|[EnrollmentProfile を削除します。](../api/intune-enrollment-enrollmentprofile-delete.md)|なし|の[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)を削除します。|
|[EnrollmentProfile を更新します。](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。|
|[setDefaultProfile アクション](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|なし|まだ文書化されていません|
|[exportMobileConfig 関数](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|モバイルの構成をエクスポートします。|
|[updateDeviceProfileAssignment アクション](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの GUID|
|displayName|String|プロファイルの名前|
|説明|String|プロファイルの説明|
|requiresUserAuthentication|Boolean|プロファイルにユーザー認証が必要なかどうかを示します|
|configurationEndpointUrl|String|登録に使用するエンドポイントの url を構成|
|enableAuthenticationViaCompanyPortal|Boolean|アップルらくらく企業ポータルではなくを使用して認証することを示します。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|セットアップ アシスタントが登録されているデバイス上の会社のポータルが必要であることを示します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




