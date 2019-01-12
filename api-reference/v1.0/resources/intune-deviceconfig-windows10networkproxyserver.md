---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4e9f727916f055fe197f98b07625b00406e16e83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921102"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ネットワーク プロキシ サーバーのポリシーです。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|address|String|プロキシ サーバーへのアドレス。 <server>\[“:”<port>\] 形式でアドレスを指定します|
|exceptions|String コレクション|プロキシ サーバーを使用できないアドレス。 システムは、このノードで指定されたもので始まるアドレスに対してプロキシ サーバーを使用しません。|
|useForLocalAddresses|Boolean|ローカル (イントラネット) アドレスにプロキシ サーバーを使用する必要があるかどうかを指定します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



