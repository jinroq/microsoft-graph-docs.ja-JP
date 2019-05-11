---
title: numberRange リソースの種類
description: 番号範囲の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8912b6a0cba8c1265060a53a8f32d9455b3bba39
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951032"
---
# <a name="numberrange-resource-type"></a>numberRange リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

番号範囲の定義。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|小数|Int32|数値 (小)|
|upperNumber|Int32|上番号|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```




