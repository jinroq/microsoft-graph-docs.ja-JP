---
title: macOSFirewallApplication リソースの種類
description: MacOS ファイアウォール アプリケーションの一覧でアプリケーションを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 536f2f596286f6b5457557f575ba018c65001bfe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835221"
---
# <a name="macosfirewallapplication-resource-type"></a>macOSFirewallApplication リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

MacOS ファイアウォール アプリケーションの一覧でアプリケーションを表します。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|bundleId|String|アプリケーションのメニューです。|
|allowsIncomingConnections|ブール型|着信接続ができるかどうか。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```





