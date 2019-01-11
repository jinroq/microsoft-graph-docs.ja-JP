---
title: updateWindowsDeviceAccountActionParameter リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3a68289aae9c3071a05a4f67d432c5e816ac7f52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809059"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a>updateWindowsDeviceAccountActionParameter リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|deviceAccount|[windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)|まだ文書化されていません|
|passwordRotationEnabled|ブール型 (Boolean)|まだ文書化されていません|
|calendarSyncEnabled|ブール型 (Boolean)|まだ文書化されていません|
|deviceAccountEmail|文字列型 (String)|まだ文書化されていません|
|exchangeServer|文字列型 (String)|まだ文書化されていません|
|sessionInitiationProtocalAddress|文字列型 (String)|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```





