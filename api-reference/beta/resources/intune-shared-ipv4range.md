---
title: iPv4Range リソースの種類
description: IPv4 の範囲定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c896eb6f9a35992d7370cf29124d8072c171eb30
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776928"
---
# <a name="ipv4range-resource-type"></a>iPv4Range リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

IPv4 の範囲定義。


[ipRange](../resources/intune-shared-iprange.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lowerAddress|文字列|小さいアドレス。|
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





