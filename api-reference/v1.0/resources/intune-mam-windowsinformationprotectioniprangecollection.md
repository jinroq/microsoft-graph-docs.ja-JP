---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2ba01b8a4385b5c06cc1e6a95441e9b7946a116d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839747"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a>windowsInformationProtectionIPRangeCollection リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 情報保護の IP 範囲のコレクション
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|displayName|文字列|表示名|
|範囲|[ipRange](../resources/intune-mam-iprange.md) コレクション|IP 範囲のコレクション|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



