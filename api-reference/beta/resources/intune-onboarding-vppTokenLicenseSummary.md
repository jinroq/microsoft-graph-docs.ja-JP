---
title: vppTokenLicenseSummary リソースの種類
description: トークンで指定されたアプリケーションのライセンスの概要です。
ms.openlocfilehash: fba888c706b21a796615bf9bc2ea79968d5ad6d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068132"
---
# <a name="vpptokenlicensesummary-resource-type"></a>vppTokenLicenseSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

トークンで指定されたアプリケーションのライセンスの概要です。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|vppTokenId|String|VPP トークンの識別子です。|
|appleId|String|特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。|
|organizationName|String|Apple ボリューム購入プログラム トークンに関連付けられている組織です。|
|availableLicenseCount|Int32|VPP のライセンスが使用可能な数です。|
|usedLicenseCount|Int32|使用中の VPP ライセンスの数。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```





