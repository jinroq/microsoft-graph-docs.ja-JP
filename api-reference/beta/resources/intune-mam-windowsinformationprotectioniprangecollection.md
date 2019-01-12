---
title: windowsInformationProtectionIPRangeCollection リソースの種類
description: Windows 情報保護の IP 範囲のコレクション
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9981b585818bb6db712b0088b2fde275179917ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911827"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a>windowsInformationProtectionIPRangeCollection リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 情報保護の IP 範囲のコレクション
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|displayName|文字列|表示名|
|範囲|[ipRange](../resources/intune-shared-iprange.md) コレクション|IP 範囲のコレクション|

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
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```





