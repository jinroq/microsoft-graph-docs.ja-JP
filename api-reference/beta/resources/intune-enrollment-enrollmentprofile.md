---
title: enrollmentProfile リソースの種類
description: EnrollmentProfile リソースでは、プレステージされて id が特定のデバイスの登録を有効にするのには事前登録を提供する必要がある構成のコレクションを表します。 ステージング済みのデバイスの id は、対応するデバイスの登録時のプロファイルの構成を適用するのには、このタイプのプロファイルに割り当てられます。
ms.openlocfilehash: 884fee5c6851e79d96cd036294e5e5485d6df66a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070132"
---
# <a name="enrollmentprofile-resource-type"></a>enrollmentProfile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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
|requiresUserAuthentication|ブール値|プロファイルにユーザー認証が必要なかどうかを示します|
|configurationEndpointUrl|String|登録に使用するエンドポイントの url を構成|
|enableAuthenticationViaCompanyPortal|ブール値|アップルらくらく企業ポータルではなくを使用して認証することを示します。|

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
  "enableAuthenticationViaCompanyPortal": true
}
```





