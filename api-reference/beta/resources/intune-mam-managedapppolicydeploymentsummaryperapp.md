---
title: managedAppPolicyDeploymentSummaryPerApp リソースの種類
description: アプリごとのポリシーの展開の概要を表します。
author: tfitzmac
ms.openlocfilehash: 8786ff0600b59a2cb729d1d7b5b4c692ab1704de
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351339"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a>managedAppPolicyDeploymentSummaryPerApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリごとのポリシーの展開の概要を表します。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|アプリの展開|
|configurationAppliedUserCount|Int32|ポリシーが適用されているユーザーの数。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```





