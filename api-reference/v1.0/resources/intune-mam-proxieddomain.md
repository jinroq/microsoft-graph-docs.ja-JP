---
title: proxiedDomain リソースの種類
description: プロキシ化されたドメイン
author: tfitzmac
ms.openlocfilehash: dc924d75bc2cf1310cb715033281f59b70abb32a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320294"
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



