---
title: osVersionCount リソースの種類
description: 各オペレーティング システムのバージョンのマルウェアとデバイスの数
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbe0d8ac149ad84ba4cd1286fb0f2303cdfb52a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410463"
---
# <a name="osversioncount-resource-type"></a>osVersionCount リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

各オペレーティング システムのバージョンのマルウェアとデバイスの数

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|osVersion|String|OS のバージョン|
|deviceCount|Int32|OS のバージョンのマルウェアとデバイスの数|
|lastUpdateDateTime|DateTimeOffset|デバイスの最後の更新のタイムスタンプは UTC でカウントします。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```




