---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed4af707320da09c9b72537168f8fd77a424c790
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258738"
---
# <a name="keyvaluepair-resource-type"></a>keyValuePair リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

カスタム設定の保存用のキーと値のペア

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|String|キーと値のペアの名前|
|value|文字列|キーと値のペアの値|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



