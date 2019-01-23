---
title: androidMinimumOperatingSystem リソースの種類
description: Android モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4328cfe06180be138b2c33840c72620efdaa277b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403127"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>androidMinimumOperatingSystem リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|v4_0|ブール型 (Boolean)|バージョン 4.0 以降。|
|v4_0_3|ブール型 (Boolean)|バージョン 4.0.3 以降。|
|v4_1|ブール型 (Boolean)|バージョン 4.1 以降。|
|v4_2|ブール型 (Boolean)|バージョン 4.2 以降。|
|v4_3|ブール型 (Boolean)|バージョン 4.3 以降。|
|v4_4|ブール型 (Boolean)|バージョン 4.4 以降。|
|v5_0|ブール型 (Boolean)|バージョン 5.0 以降。|
|v5_1|ブール型 (Boolean)|バージョン 5.1 以降。|
|v6_0|Boolean|6.0 またはそれ以降のバージョンです。|
|v7_0|Boolean|7.0 またはそれ以降のバージョンです。|
|v7_1|Boolean|7.1 以降のバージョンです。|
|v8_0|ブール型 (Boolean)|バージョン 8.0 以降。|
|v8_1|ブール型 (Boolean)|8.1 またはそれ以降のバージョンです。|
|v9_0|ブール型 (Boolean)|バージョン 9.0 以降。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true,
  "v6_0": true,
  "v7_0": true,
  "v7_1": true,
  "v8_0": true,
  "v8_1": true,
  "v9_0": true
}
```




