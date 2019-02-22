---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a8feecabeca3cfc916c0bd3ce1b87cab3a68809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160796"
---
# <a name="keyvaluepair-resource-type"></a>keyValuePair リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

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




