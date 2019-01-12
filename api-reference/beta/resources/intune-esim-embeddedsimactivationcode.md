---
title: embeddedSIMActivationCode リソースの種類
description: 携帯電話会社で提供される、埋め込みコードの SIM のアクティブ化します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af8bf020953dbc014f42aa6d363d3ca9e30db8a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987406"
---
# <a name="embeddedsimactivationcode-resource-type"></a>embeddedSIMActivationCode リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

携帯電話会社で提供される、埋め込みコードの SIM のアクティブ化します。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|integratedCircuitCardIdentifier|String|この集積回路カードの識別子 (ICCID) では、携帯電話会社によって提供されると、SIM の有効化コードが埋め込まれています。
入力が次の正規表現に一致する必要があります: '^\[0-9\]{19}\[0-9\]?$' です。|
|matchingIdentifier|String|GSMA アソシエーション SGP.22 RSP 技術仕様セクション 4.1 で指定されている MatchingIdentifier (MatchingID)。
入力が次の正規表現に一致する必要があります: ' ^\[a-zA-Z0-9\-\]* $' です。|
|smdpPlusServerAddress|String|SM の完全修飾ドメイン名-DP + GSM 関連 SPG.22 RSP の技術的な仕様で指定されているサーバーです。
入力が次の正規表現に一致する必要があります: ' ^ (\[、-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) *\.) +\[a, A-Z\]{2,}$' です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```





