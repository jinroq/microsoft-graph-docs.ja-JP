---
title: iPv4Range リソースの種類
description: IPv4 の範囲定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14cb0d88013b13f57b186f5388d5ac89f60db043
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465525"
---
# <a name="ipv4range-resource-type"></a>iPv4Range リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

IPv4 の範囲定義。


[ipRange](../resources/intune-mam-iprange.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lowerAddress|String|小さいアドレス。|
|upperAddress|文字列型 (String)|上住所|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



