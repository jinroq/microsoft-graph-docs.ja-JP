---
title: rgbColor リソースの種類
description: RGB 色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2222d7142ea033a8db2c2ce263da04c3b33153
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524555"
---
# <a name="rgbcolor-resource-type"></a>rgbColor リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

RGB 色。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|r|バイト型 (Byte)|赤の値|
|g|バイト型 (Byte)|緑の値|
|b|バイト型 (Byte)|青の値|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```



