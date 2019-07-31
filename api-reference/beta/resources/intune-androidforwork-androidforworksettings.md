---
title: androidForWorkSettings リソース タイプ
description: Android for Work の設定です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df1efa63e2894dccc0208ec1bca5aef8b75df4b2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005619"
---
# <a name="androidforworksettings-resource-type"></a>androidForWorkSettings リソース タイプ

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android for Work の設定です。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update androidForWorkSettings](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトのプロパティを更新します。|
|[requestSignupUrl action](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|String|まだ文書化されていません|
|[completeSignup action](../api/intune-androidforwork-androidforworksettings-completesignup.md)|なし|まだ文書化されていません|
|[syncApps action](../api/intune-androidforwork-androidforworksettings-syncapps.md)|なし|まだ文書化されていません|
|[unbind action](../api/intune-androidforwork-androidforworksettings-unbind.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Android for Work の設定の識別子|
|bindStatus|[Androidforwork Bindstatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|Google EMM API を使用して、テナントの状態をバインドします。 使用可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。|
|lastAppSyncDateTime|DateTimeOffset|アプリ同期の最終完了時刻|
|lastAppSyncStatus|[Androidforwork Syncstatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|最後のアプリケーションの同期結果。 使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。|
|ownerUserPrincipalName|String|エンタープライズを作成した所有者の UPN|
|ownerOrganizationName|String|Android for Work のオンボーディング時に使用される組織名|
|lastModifiedDateTime|DateTimeOffset|Android for Work の設定の最終変更時刻|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Android for Work デバイス管理にデバイスを登録できるユーザーを示します。 使用可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。|
|targetGroupIds|String コレクション|enrollmentTarget が「Targeted」に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。|
|deviceOwnerManagementEnabled|Boolean|CloudDPC を使用した Android デバイス所有者の管理に、このアカウントが flighting になるかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true
}
```





