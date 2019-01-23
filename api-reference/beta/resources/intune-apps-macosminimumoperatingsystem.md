---
title: macOSMinimumOperatingSystem リソースの種類
description: MacOS アプリケーションに必要な最低限のオペレーティング システムです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1b5bb3c31f876cb7444ff90cad5060c08d2f60b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425926"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>macOSMinimumOperatingSystem リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS アプリケーションに必要な最低限のオペレーティング システムです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|v10_7|Boolean|Mac OS 10.7 以降です。|
|v10_8|Boolean|Mac OS 10.8 以降です。|
|v10_9|Boolean|Mac OS 10.9 以降です。|
|v10_10|Boolean|Mac OS 10.10 以降です。|
|v10_11|Boolean|Mac OS 10.11 またはそれ以降です。|
|v10_12|Boolean|Mac OS 10.12 以降です。|
|v10_13|Boolean|Mac OS 10.13 またはそれ以降です。|

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




