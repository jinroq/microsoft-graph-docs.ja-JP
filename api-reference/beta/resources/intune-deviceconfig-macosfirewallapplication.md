---
title: macOSFirewallApplication リソースの種類
description: MacOS ファイアウォールアプリケーションの一覧にあるアプリを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a22914ba0af21418b593015995b6d7665ae3bc3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992200"
---
# <a name="macosfirewallapplication-resource-type"></a>macOSFirewallApplication リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS ファイアウォールアプリケーションの一覧にあるアプリを表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|bundleId|String|アプリケーションの BundleId。|
|allowsIncomingConnections|Boolean|受信接続を許可するかどうかを指定します。|

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





