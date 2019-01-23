---
title: windowsMinimumOperatingSystem リソースの種類
description: Windows モバイル アプリに必要な最小オペレーティング システム。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c293e7490df1e7a6c53628b49440a050ee21a39
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395819"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows モバイル アプリに必要な最小オペレーティング システム。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|v8_0|ブール型 (Boolean)|Windows バージョン 8.0 以降。|
|v8_1|ブール型 (Boolean)|Windows バージョン 8.1 以降。|
|v10_0|ブール型 (Boolean)|Windows バージョン 10.0 以降。|
|v10_1607|Boolean|Windows 10 1607 以降です。|
|v10_1703|Boolean|10 1703 の Windows またはそれ以降です。|
|v10_1709|Boolean|10 1709 の Windows またはそれ以降です。|
|v10_1803|Boolean|10 1803 の Windows またはそれ以降です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true,
  "v10_1607": true,
  "v10_1703": true,
  "v10_1709": true,
  "v10_1803": true
}
```




