---
title: windows10NetworkProxyServer リソースの種類
description: ネットワーク プロキシ サーバーのポリシーです。
ms.openlocfilehash: 4e2e995c8d66249e5c742343f74e18e87337bfaa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071991"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ネットワーク プロキシ サーバーのポリシーです。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
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




