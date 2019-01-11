---
title: macOSMinimumOperatingSystem リソースの種類
description: MacOS アプリケーションに必要な最低限のオペレーティング システムです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 21f557ebd3fbc1ae5e86a1991eb1a0207a902ce2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862091"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>macOSMinimumOperatingSystem リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

MacOS アプリケーションに必要な最低限のオペレーティング システムです。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|v10_7|ブール型|Mac OS 10.7 以降です。|
|v10_8|ブール型|Mac OS 10.8 以降です。|
|v10_9|ブール型|Mac OS 10.9 以降です。|
|v10_10|ブール型|Mac OS 10.10 以降です。|
|v10_11|ブール型|Mac OS 10.11 またはそれ以降です。|
|v10_12|ブール型|Mac OS 10.12 以降です。|
|v10_13|ブール型|Mac OS 10.13 またはそれ以降です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSMinimumOperatingSystem",
  "v10_7": true,
  "v10_8": true,
  "v10_9": true,
  "v10_10": true,
  "v10_11": true,
  "v10_12": true,
  "v10_13": true
}
```





