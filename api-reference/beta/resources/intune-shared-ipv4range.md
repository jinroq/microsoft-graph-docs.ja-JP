---
title: iPv4Range リソースの種類
description: IPv4 の範囲定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c740cc94965ae41a857aa2c6ccb1394e161e6866
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996002"
---
# <a name="ipv4range-resource-type"></a>iPv4Range リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

IPv4 の範囲定義。


[ipRange](../resources/intune-shared-iprange.md) からの継承

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





