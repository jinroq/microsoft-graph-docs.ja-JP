---
title: managedDeviceMobileAppConfigurationUserSummary リソースの種類
description: MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e919a758d68c847b1ff4fe6be08890bbcf2ab902
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977186"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a>managedDeviceMobileAppConfigurationUserSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedDeviceMobileAppConfigurationUserSummary の取得](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedDeviceMobileAppConfigurationUserSummary の更新](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|pendingCount|Int32|保留中のユーザーの数|
|notApplicableCount|Int32|適用されないユーザーの数|
|successCount|Int32|成功したユーザーの数|
|errorCount|Int32|エラー ユーザーの数|
|failedCount|Int32|失敗したユーザーの数|
|conflictCount|Int32|競合しているユーザーの数|
|lastUpdateDateTime|DateTimeOffset|最終更新時刻|
|configurationVersion|Int32|対象の概要に関するポリシーのバージョン|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





