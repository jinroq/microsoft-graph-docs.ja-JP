---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49afbb3383035711bc950a9a7226a354ae78f0e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920430"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>deviceExchangeAccessStateSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスの Exchange アクセス状態の要約
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|allowedDeviceCount|Int32|Exchange アクセス状態が Allowed のデバイスの総数です。|
|blockedDeviceCount|Int32|Exchange アクセス状態が Blocked のデバイスの総数です。|
|quarantinedDeviceCount|Int32|Exchange アクセス状態が Quarantined のデバイスの総数です。|
|unknownDeviceCount|Int32|Exchange アクセス状態が Unknown のデバイスの総数です。|
|unavailableDeviceCount|Int32|Exchange アクセス状態を検出できなかったデバイスの総数です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```





