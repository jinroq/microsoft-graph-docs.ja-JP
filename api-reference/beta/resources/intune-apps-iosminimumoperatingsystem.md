---
title: iosMinimumOperatingSystem リソースの種類
description: iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4a97932c76a737aa1a98321feb429244228c97d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406942"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>iosMinimumOperatingSystem リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|v8_0|ブール型 (Boolean)|バージョン 8.0 以降。|
|v9_0|ブール型 (Boolean)|バージョン 9.0 以降。|
|v10_0|ブール型 (Boolean)|バージョン 10.0 以降。|
|v11_0|ブール型 (Boolean)|バージョン 11.0 以降。|
|v12_0|Boolean|12.0 またはそれ以降のバージョンです。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```




