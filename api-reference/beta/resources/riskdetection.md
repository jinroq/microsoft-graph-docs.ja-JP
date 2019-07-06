---
title: riskDetection リソースの種類
description: AzureAD テナントのすべてのリスクの検出を表します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 07a3a76f2ec2a4c3e1536f4b4d61e52417c2053c
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576467"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="31f5c-103">riskDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31f5c-103">riskDetection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31f5c-104">Azure AD テナントの検出されたリスクに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-104">Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="31f5c-105">Azure AD は、さまざまなシグナルやマシン学習に基づいて、[ユーザーのリスク](riskyuser.md)とアプリまたはユーザー[のサインイン](signin.md)リスクを継続的に評価します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-105">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="31f5c-106">この API は、Azure AD 環境のすべてのリスク検出へのプログラムによるアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-106">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="31f5c-107">リスクイベントの詳細については、「 [Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31f5c-107">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

>[!NOTE]
><span data-ttu-id="31f5c-108">リスク検出 API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="31f5c-108">You must have an Azure AD Premium P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="31f5c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="31f5c-109">Methods</span></span>

| <span data-ttu-id="31f5c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="31f5c-110">Method</span></span>   | <span data-ttu-id="31f5c-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="31f5c-111">Return Type</span></span>|<span data-ttu-id="31f5c-112">説明</span><span class="sxs-lookup"><span data-stu-id="31f5c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31f5c-113">リスト riskDetection</span><span class="sxs-lookup"><span data-stu-id="31f5c-113">List riskDetection</span></span>](../api/riskdetection-list.md) | <span data-ttu-id="31f5c-114">[riskDetection](riskdetection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="31f5c-114">[riskDetection](riskdetection.md) collection</span></span>|<span data-ttu-id="31f5c-115">リスクの検出とそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-115">List risk detections and their properties.</span></span>|
|[<span data-ttu-id="31f5c-116">RiskDetection を取得する</span><span class="sxs-lookup"><span data-stu-id="31f5c-116">Get riskDetection</span></span>](../api/riskdetection-get.md) | [<span data-ttu-id="31f5c-117">riskDetection</span><span class="sxs-lookup"><span data-stu-id="31f5c-117">riskDetection</span></span>](riskdetection.md)|<span data-ttu-id="31f5c-118">特定の危険な検出とそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-118">Get a specific risky detection and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="31f5c-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31f5c-119">Properties</span></span>

| <span data-ttu-id="31f5c-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31f5c-120">Property</span></span>   | <span data-ttu-id="31f5c-121">型</span><span class="sxs-lookup"><span data-stu-id="31f5c-121">Type</span></span>|<span data-ttu-id="31f5c-122">説明</span><span class="sxs-lookup"><span data-stu-id="31f5c-122">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="31f5c-123">リスク検出の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="31f5c-123">Unique ID of the risk detection.</span></span> |
|`requestId`|`string`|<span data-ttu-id="31f5c-124">リスクの検出に関連付けられているサインインの要求 ID。</span><span class="sxs-lookup"><span data-stu-id="31f5c-124">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="31f5c-125">リスクの検出がサインインに関連付けられていない場合、このプロパティは null になります。</span><span class="sxs-lookup"><span data-stu-id="31f5c-125">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|`correlationId`|`string`|<span data-ttu-id="31f5c-126">リスクの検出に関連付けられているサインインの関連付け ID。</span><span class="sxs-lookup"><span data-stu-id="31f5c-126">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="31f5c-127">リスクの検出がサインインに関連付けられていない場合、このプロパティは null になります。</span><span class="sxs-lookup"><span data-stu-id="31f5c-127">This property is null if the risk detection is not associated with a sign-in.</span></span> |
|`riskType`|`riskEventType`|<span data-ttu-id="31f5c-128">検出されたリスクイベントの種類。</span><span class="sxs-lookup"><span data-stu-id="31f5c-128">The type of risk event detected.</span></span> <span data-ttu-id="31f5c-129">使用可能な値は、unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、、、investigationsThreatIntelligence、genericadminConfirmedUserCompromised、Mcasimwait トラベル、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、および Unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="31f5c-129">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genericadminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, and unknownFutureValue.</span></span> |
|`riskState`|`riskState`|<span data-ttu-id="31f5c-130">検出されたリスクの高いユーザーまたはサインインの状態。</span><span class="sxs-lookup"><span data-stu-id="31f5c-130">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="31f5c-131">使用可能な値は、none、confirmedSafe、修復、消さ、atRisk、confirmedCompromised、および Unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="31f5c-131">The possible values are none, confirmedSafe, remediated, dismissed, atRisk, confirmedCompromised, and unknownFutureValue.</span></span> |
|`riskLevel`|`riskLevel`|<span data-ttu-id="31f5c-132">検出されたリスクのレベル。</span><span class="sxs-lookup"><span data-stu-id="31f5c-132">Level of the detected risk.</span></span> <span data-ttu-id="31f5c-133">使用可能な値は、low、medium、high、hidden、none、Unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="31f5c-133">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span> |
|`riskDetail`|`riskDetail`|<span data-ttu-id="31f5c-134">検出されたリスクの詳細。</span><span class="sxs-lookup"><span data-stu-id="31f5c-134">Details of the detected risk.</span></span> <span data-ttu-id="31f5c-135">使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、Unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="31f5c-135">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span> |
|`source`|`string`|<span data-ttu-id="31f5c-136">リスク検出のソース。</span><span class="sxs-lookup"><span data-stu-id="31f5c-136">Source of the risk detection.</span></span> <span data-ttu-id="31f5c-137">たとえば、"activeDirectory" を使用します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-137">For example, "activeDirectory".</span></span> |
|`detectionTimingType`|`riskDetectionTimingType`|<span data-ttu-id="31f5c-138">検出されたリスクのタイミング (リアルタイム/オフライン)。</span><span class="sxs-lookup"><span data-stu-id="31f5c-138">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="31f5c-139">指定可能な値は、定義されていません。リアルタイム、nearRealtime、offline、Unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="31f5c-139">The possible values are notDefined, realtime, nearRealtime, offline, unknownFutureValue.</span></span> |
|`activity`|`activityType`|<span data-ttu-id="31f5c-140">検出されたリスクがリンクされているアクティビティの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-140">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="31f5c-141">使用可能な値は、サインイン、ユーザー、Unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="31f5c-141">The possible values are signin, user, unknownFutureValue.</span></span> |
|`tokenIssuerType`|`tokenIssuerType`|<span data-ttu-id="31f5c-142">検出されたサインインリスクのトークン発行元の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-142">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="31f5c-143">使用可能な値は、AzureAD、ADFederationServices、および Unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="31f5c-143">The possible values are AzureAD, ADFederationServices, and unknownFutureValue.</span></span> |
|`ipAddress`|`string`|<span data-ttu-id="31f5c-144">リスクが発生したクライアントの IP アドレスを提供します。</span><span class="sxs-lookup"><span data-stu-id="31f5c-144">Provides the IP address of the client from where the risk occurred.</span></span> |
|`location`|[`signInLocation`](signinlocation.md)|<span data-ttu-id="31f5c-145">サインインの場所。</span><span class="sxs-lookup"><span data-stu-id="31f5c-145">Location of the sign-in.</span></span> |
|`activityDateTime`|`datetimeoffset`|<span data-ttu-id="31f5c-146">危険な活動が発生した日時。</span><span class="sxs-lookup"><span data-stu-id="31f5c-146">Date and time that the risky activity occurred.</span></span> |
|`detectedDateTime`|`datetimeoffset`|<span data-ttu-id="31f5c-147">リスクが検出された日時。</span><span class="sxs-lookup"><span data-stu-id="31f5c-147">Date and time that the risk was detected.</span></span> |
|`lastUpdatedDateTime`|`datetime`|<span data-ttu-id="31f5c-148">リスク検出が最後に更新された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="31f5c-148">Date and time that the risk detection was last updated.</span></span> |
|`userId`|`string`|<span data-ttu-id="31f5c-149">ユーザーの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="31f5c-149">Unique ID of the user.</span></span> |
|`userDisplayName`|`string`|<span data-ttu-id="31f5c-150">ユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="31f5c-150">Name of the user.</span></span> |
|`userPrincipalName`|`string`|<span data-ttu-id="31f5c-151">ユーザーのユーザープリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="31f5c-151">The user principal name (UPN) of the user.</span></span> |
|`additionalInfo`|`string`|<span data-ttu-id="31f5c-152">JSON 形式でのリスクの検出に関連付けられている追加情報。</span><span class="sxs-lookup"><span data-stu-id="31f5c-152">Additional information associated with the risk detection in JSON format.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31f5c-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31f5c-153">JSON representation</span></span>

<span data-ttu-id="31f5c-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31f5c-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
