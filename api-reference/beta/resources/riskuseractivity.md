---
title: riskUserActivity リソースの種類
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 258cd61b55d0ac8d19f83682fe34d53cc4b233b0
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/09/2019
ms.locfileid: "31688508"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="2209c-102">riskUserActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2209c-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="2209c-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2209c-103">Properties</span></span>

| <span data-ttu-id="2209c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2209c-104">Property</span></span>       | <span data-ttu-id="2209c-105">型</span><span class="sxs-lookup"><span data-stu-id="2209c-105">Type</span></span>    |<span data-ttu-id="2209c-106">説明</span><span class="sxs-lookup"><span data-stu-id="2209c-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2209c-107">eventTypes</span><span class="sxs-lookup"><span data-stu-id="2209c-107">eventTypes</span></span> | <span data-ttu-id="2209c-108">riskEventType コレクション</span><span class="sxs-lookup"><span data-stu-id="2209c-108">riskEventType collection</span></span> |<span data-ttu-id="2209c-109">使用可能な値は、unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、つの最小値の資格情報、investigationsThreatIntelligence、generic、adminConfirmedUserCompromised、mcasimtimed トラベル、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="2209c-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="2209c-110">細部</span><span class="sxs-lookup"><span data-stu-id="2209c-110">detail</span></span>     | <span data-ttu-id="2209c-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2209c-111">riskDetail</span></span>  | <span data-ttu-id="2209c-112">使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="2209c-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2209c-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2209c-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": [{"@odata.type":"microsoft.graph.riskEventType"}],
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
