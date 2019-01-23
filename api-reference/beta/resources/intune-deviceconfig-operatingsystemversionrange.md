---
title: operatingSystemVersionRange リソースの種類
description: オペレーティング システムのバージョンの範囲です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aaac008b013a8bf2cfd1a88d1fab06a523abb949
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398528"
---
# <a name="operatingsystemversionrange-resource-type"></a>operatingSystemVersionRange リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

オペレーティング システムのバージョンの範囲です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|説明|String|この範囲 (有効 1702 のビルドなど) の説明|
|lowestVersion|String|最小包括的なバージョンをこの範囲に含まれています。|
|highestVersion|String|この範囲に含まれている最高の包括的なバージョンです。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```




