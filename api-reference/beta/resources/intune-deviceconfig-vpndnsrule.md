---
title: vpnDnsRule リソースの種類
description: VPN の DNS ルール定義します。
author: tfitzmac
ms.openlocfilehash: 7be94c48dafd4352938ac2c63ab1af66c65ea098
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351164"
---
# <a name="vpndnsrule-resource-type"></a>vpnDnsRule リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

VPN の DNS ルール定義します。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|名前|String|名前です。|
|サーバー|String コレクション|サーバーです。|
|proxyServerUri|String|プロキシ サーバーの Uri。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String"
}
```





