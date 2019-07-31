---
title: riskUserActivity リソースの種類
description: author
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4b33d4f9344f8031076f00b1b442b882fffe6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965356"
---
# <a name="riskuseractivity-resource-type"></a>riskUserActivity リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>プロパティ

| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
| eventTypes | riskEventType コレクション |使用可能な値は、unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、つの最小値の資格情報、investigationsThreatIntelligence、generic、adminConfirmedUserCompromised、Mcasimtimed トラベル、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、Unknownfuturevalue という。  |
| 細部     | riskDetail  | 使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、Unknownfuturevalue という。  |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": ["String"],
    "detail": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "",
  "tocPath": "",
  "suppressions": []
}
-->
