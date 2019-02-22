---
title: しましたリソースの種類
description: しましたリソースは、事前登録を提供する必要がある構成のコレクションを表します。これにより、id が事前にステージングされている特定のデバイスを登録することができます。 事前に展開されたデバイス id は、対応するデバイスの登録時にプロファイルの構成を適用するために、この種類のプロファイルに割り当てられます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d8947864611ac2c0d26256a5d739d41b86c383f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151178"
---
# <a name="enrollmentprofile-resource-type"></a>しましたリソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

しましたリソースは、事前登録を提供する必要がある構成のコレクションを表します。これにより、id が事前にステージングされている特定のデバイスを登録することができます。 事前に展開されたデバイス id は、対応するデバイスの登録時にプロファイルの構成を適用するために、この種類のプロファイルに割り当てられます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[しました](../resources/intune-enrollment-enrollmentprofile.md)コレクション|[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[しましたを取得する](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[しましたを作成する](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|新しい[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。|
|[しましたの削除](../api/intune-enrollment-enrollmentprofile-delete.md)|なし|[しました](../resources/intune-enrollment-enrollmentprofile.md)を削除します。|
|[しましたの更新](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。|
|[setDefaultProfile アクション](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|なし|まだ文書化されていません|
|[exportmobileconfig 関数](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|モバイル構成をエクスポートします。|
|[updateDeviceProfileAssignment アクション](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの GUID|
|displayName|String|プロファイルの名前|
|説明|String|プロファイルの説明|
|requiresUserAuthentication|ブール値|プロファイルにユーザー認証が必要かどうかを示します|
|configurationendpointurl|String|登録に使用する構成エンドポイント url|
|enableAuthenticationViaCompanyPortal|ブール値|会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|ブール値|セットアップアシスタントの登録済みデバイスで会社のポータルが必要であることを示します。|

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




