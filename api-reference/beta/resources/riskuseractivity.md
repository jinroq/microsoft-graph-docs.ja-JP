---
title: riskUserActivity リソースの種類
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1685c58697f9de52e209d508c1ec104b9c044e8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343564"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="6af98-102">riskUserActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6af98-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="6af98-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6af98-103">Properties</span></span>

| <span data-ttu-id="6af98-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6af98-104">Property</span></span>       | <span data-ttu-id="6af98-105">型</span><span class="sxs-lookup"><span data-stu-id="6af98-105">Type</span></span>    |<span data-ttu-id="6af98-106">説明</span><span class="sxs-lookup"><span data-stu-id="6af98-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6af98-107">eventTypes</span><span class="sxs-lookup"><span data-stu-id="6af98-107">eventTypes</span></span> | <span data-ttu-id="6af98-108">riskEventType コレクション</span><span class="sxs-lookup"><span data-stu-id="6af98-108">riskEventType collection</span></span> |<span data-ttu-id="6af98-109">使用可能な値は、unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、つの最小値の資格情報、investigationsThreatIntelligence、generic、adminConfirmedUserCompromised、mcasimtimed トラベル、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="6af98-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="6af98-110">細部</span><span class="sxs-lookup"><span data-stu-id="6af98-110">detail</span></span>     | <span data-ttu-id="6af98-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="6af98-111">riskDetail</span></span>  | <span data-ttu-id="6af98-112">使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="6af98-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6af98-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6af98-113">JSON representation</span></span>

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
