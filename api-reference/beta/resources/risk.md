---
title: リソースの種類のリスク
description: レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 48fda9624e45072240bc694b8b5e152fe3ef0764
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524822"
---
# <a name="risk-resource-type"></a><span data-ttu-id="b5444-103">リソースの種類のリスク</span><span class="sxs-lookup"><span data-stu-id="b5444-103">risk resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5444-104">レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。</span><span class="sxs-lookup"><span data-stu-id="b5444-104">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="b5444-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5444-105">Properties</span></span>

| <span data-ttu-id="b5444-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5444-106">Property</span></span>   | <span data-ttu-id="b5444-107">型</span><span class="sxs-lookup"><span data-stu-id="b5444-107">Type</span></span>|<span data-ttu-id="b5444-108">説明</span><span class="sxs-lookup"><span data-stu-id="b5444-108">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="b5444-109">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b5444-109">riskDetail</span></span>|<span data-ttu-id="b5444-110">危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。</span><span class="sxs-lookup"><span data-stu-id="b5444-110">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b5444-111">可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b5444-111">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="b5444-112">値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。</span><span class="sxs-lookup"><span data-stu-id="b5444-112">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="b5444-113">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b5444-113">riskLevel</span></span>|<span data-ttu-id="b5444-114">危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。</span><span class="sxs-lookup"><span data-stu-id="b5444-114">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b5444-115">可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b5444-115">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="b5444-116">値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。</span><span class="sxs-lookup"><span data-stu-id="b5444-116">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="b5444-117">riskLeve</span><span class="sxs-lookup"><span data-stu-id="b5444-117">riskLeve</span></span>|<span data-ttu-id="b5444-118">サインイン中に、(すなわち、リアルタイムのリスク イベントに基づいて) には、サインイン用のリスクのレベルを提供します。</span><span class="sxs-lookup"><span data-stu-id="b5444-118">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="b5444-119">可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b5444-119">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="b5444-120">値`hidden`サインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。</span><span class="sxs-lookup"><span data-stu-id="b5444-120">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="b5444-121">riskState</span><span class="sxs-lookup"><span data-stu-id="b5444-121">riskState</span></span>|<span data-ttu-id="b5444-122">危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。</span><span class="sxs-lookup"><span data-stu-id="b5444-122">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b5444-123">使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b5444-123">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b5444-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5444-124">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/risk.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
