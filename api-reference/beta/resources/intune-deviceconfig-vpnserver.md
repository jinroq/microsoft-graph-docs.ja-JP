---
title: vpnServer のリソースの種類
description: VPN サーバーの定義です。
author: tfitzmac
ms.openlocfilehash: a8f0e6bd38f243d0066da231ef07d1723961987b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328778"
---
# <a name="vpnserver-resource-type"></a>vpnServer のリソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

VPN サーバーの定義です。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|説明|String|説明。|
|address|String|アドレス (IP アドレス、FQDN、または URL)|
|isDefaultServer|ブール型|既定のサーバーです。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```





