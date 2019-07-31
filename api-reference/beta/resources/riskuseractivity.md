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
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="8a718-103">riskUserActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a718-103">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="8a718-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a718-104">Properties</span></span>

| <span data-ttu-id="8a718-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a718-105">Property</span></span>       | <span data-ttu-id="8a718-106">型</span><span class="sxs-lookup"><span data-stu-id="8a718-106">Type</span></span>    |<span data-ttu-id="8a718-107">説明</span><span class="sxs-lookup"><span data-stu-id="8a718-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a718-108">eventTypes</span><span class="sxs-lookup"><span data-stu-id="8a718-108">eventTypes</span></span> | <span data-ttu-id="8a718-109">riskEventType コレクション</span><span class="sxs-lookup"><span data-stu-id="8a718-109">riskEventType collection</span></span> |<span data-ttu-id="8a718-110">使用可能な値は、unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、つの最小値の資格情報、investigationsThreatIntelligence、generic、adminConfirmedUserCompromised、Mcasimtimed トラベル、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、Unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="8a718-110">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="8a718-111">細部</span><span class="sxs-lookup"><span data-stu-id="8a718-111">detail</span></span>     | <span data-ttu-id="8a718-112">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8a718-112">riskDetail</span></span>  | <span data-ttu-id="8a718-113">使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、Unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="8a718-113">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8a718-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a718-114">JSON representation</span></span>

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
