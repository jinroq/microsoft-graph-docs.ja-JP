---
title: リソースの種類のリスク
description: レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 6f8fb05b39c14e3d56ddff211a5d35d77b87b814
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927269"
---
# <a name="risk-resource-type"></a><span data-ttu-id="3e442-103">リソースの種類のリスク</span><span class="sxs-lookup"><span data-stu-id="3e442-103">risk resource type</span></span>

> <span data-ttu-id="3e442-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e442-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e442-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e442-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e442-106">レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。</span><span class="sxs-lookup"><span data-stu-id="3e442-106">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="3e442-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e442-107">Properties</span></span>

| <span data-ttu-id="3e442-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e442-108">Property</span></span>   | <span data-ttu-id="3e442-109">種類</span><span class="sxs-lookup"><span data-stu-id="3e442-109">Type</span></span>|<span data-ttu-id="3e442-110">説明</span><span class="sxs-lookup"><span data-stu-id="3e442-110">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="3e442-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="3e442-111">riskDetail</span></span>|<span data-ttu-id="3e442-112">危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。</span><span class="sxs-lookup"><span data-stu-id="3e442-112">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3e442-113">可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3e442-113">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="3e442-114">値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。</span><span class="sxs-lookup"><span data-stu-id="3e442-114">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="3e442-115">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3e442-115">riskLevel</span></span>|<span data-ttu-id="3e442-116">危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。</span><span class="sxs-lookup"><span data-stu-id="3e442-116">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3e442-117">可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3e442-117">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="3e442-118">値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。</span><span class="sxs-lookup"><span data-stu-id="3e442-118">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="3e442-119">riskLeve</span><span class="sxs-lookup"><span data-stu-id="3e442-119">riskLeve</span></span>|<span data-ttu-id="3e442-120">サインイン中に、(すなわち、リアルタイムのリスク イベントに基づいて) には、サインイン用のリスクのレベルを提供します。</span><span class="sxs-lookup"><span data-stu-id="3e442-120">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="3e442-121">可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3e442-121">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="3e442-122">値`hidden`サインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。</span><span class="sxs-lookup"><span data-stu-id="3e442-122">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="3e442-123">riskState</span><span class="sxs-lookup"><span data-stu-id="3e442-123">riskState</span></span>|<span data-ttu-id="3e442-124">危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。</span><span class="sxs-lookup"><span data-stu-id="3e442-124">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3e442-125">可能な値: `none`、 `confirmedSafe`、 `remediated`、 `dismissed`、 `atRisk`、 `confirmedCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3e442-125">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e442-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e442-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
    "stateDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
    "riskLevelAggregated":  {"@odata.type": "microsoft.graph.riskLevel"},
    "riskLevelDuringSignIn":  {"@odata.type": "microsoft.graph.riskLevel"},
    "state":  {"@odata.type": "microsoft.graph.riskState"}
  }
  ```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
