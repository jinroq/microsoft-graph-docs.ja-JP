---
title: macOSMinimumOperatingSystem リソースの種類
description: MacOS アプリに必要な最小限のオペレーティングシステム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 455c9ce625bc36b1f3423cba2a7538d1d912f6ff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005437"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>macOSMinimumOperatingSystem リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS アプリに必要な最小限のオペレーティングシステム。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|v10_7|Boolean|Mac OS 10.7 以降。|
|v10_8|Boolean|Mac OS 10.8 以降。|
|v10_9|Boolean|Mac OS 10.9 以降。|
|v10_10|Boolean|Mac OS 10.10 以降。|
|v10_11|Boolean|Mac OS 10.11 以降。|
|v10_12|Boolean|Mac OS 10.12 以降。|
|v10_13|Boolean|Mac OS 10.13 以降。|

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





