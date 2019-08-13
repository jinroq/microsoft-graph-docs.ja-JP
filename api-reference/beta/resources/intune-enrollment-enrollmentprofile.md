---
title: しましたリソースの種類
description: しましたリソースは、事前登録を提供する必要がある構成のコレクションを表します。これにより、id が事前にステージングされている特定のデバイスを登録することができます。 事前に展開されたデバイス id は、対応するデバイスの登録時にプロファイルの構成を適用するために、この種類のプロファイルに割り当てられます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 623979d78a43ede047db90f722f4a160fb22f4ad
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327990"
---
# <a name="enrollmentprofile-resource-type"></a>しましたリソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

しましたリソースは、事前登録を提供する必要がある構成のコレクションを表します。これにより、id が事前にステージングされている特定のデバイスを登録することができます。 事前に展開されたデバイス id は、対応するデバイスの登録時にプロファイルの構成を適用するために、この種類のプロファイルに割り当てられます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[しました](../resources/intune-enrollment-enrollmentprofile.md)コレクション|[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[しましたを取得する](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[しましたを作成する](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|新しい[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。|
|[しましたの削除](../api/intune-enrollment-enrollmentprofile-delete.md)|None|[しました](../resources/intune-enrollment-enrollmentprofile.md)を削除します。|
|[しましたの更新](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。|
|[setDefaultProfile アクション](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|なし|まだ文書化されていません|
|[exportMobileConfig 関数](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|モバイル構成をエクスポートします。|
|[updateDeviceProfileAssignment アクション](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|オブジェクトの GUID|
|displayName|String|プロファイルの名前|
|description|String|プロファイルの説明|
|requiresUserAuthentication|Boolean|プロファイルにユーザー認証が必要かどうかを示します|
|configurationEndpointUrl|String|登録に使用する構成エンドポイント url|
|enableAuthenticationViaCompanyPortal|Boolean|会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|セットアップアシスタントの登録済みデバイスで会社のポータルが必要であることを示します。|

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



