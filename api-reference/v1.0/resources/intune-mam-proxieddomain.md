---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eff345414531b0ddda1600bb567aacd4a5436602
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871114"
---
# <a name="proxieddomain-resource-type"></a>proxiedDomain リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

プロキシ化されたドメイン
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ipAddressOrFQDN|文字列|IP アドレスまたは FQDN|
|プロキシ|文字列|プロキシ IP|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



