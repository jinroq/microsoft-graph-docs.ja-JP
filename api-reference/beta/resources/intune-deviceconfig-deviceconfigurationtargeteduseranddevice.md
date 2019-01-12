---
title: deviceConfigurationTargetedUserAndDevice リソースの種類
description: 競合デバイスの構成のポリシーのセットの概要です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 234cc9c909875d835ba54709f30f1ca306eb0954
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947967"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>deviceConfigurationTargetedUserAndDevice リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

競合デバイスの構成のポリシーのセットの概要です。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|deviceId|String|チェックインで、デバイスの id です。|
|deviceName|String|チェックインで、デバイスの名前。|
|userId|String|チェックインでユーザーの id です。|
|userDisplayName|String|チェックインでユーザーの表示名|
|userPrincipalName|String|チェックインのユーザーの UPN。|
|lastCheckinDateTime|DateTimeOffset|このユーザー/デバイス ・ ペアの最後のチェックインの時間です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





