---
title: riskyUsers リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。 この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 27c189a81d6ba4e088c1242acfd2cf0d0f5c56c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515714"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="d0303-105">riskyUsers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0303-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0303-106">危険にさらされている Azure AD ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="d0303-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="d0303-107">Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。</span><span class="sxs-lookup"><span data-stu-id="d0303-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="d0303-108">この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="d0303-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="d0303-109">**注:** この API には、Azure AD プレミアム P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="d0303-109">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="d0303-110">リスク イベントの詳細については、 [Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0303-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="d0303-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0303-111">Methods</span></span>

| <span data-ttu-id="d0303-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0303-112">Method</span></span>   | <span data-ttu-id="d0303-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d0303-113">Return Type</span></span>|<span data-ttu-id="d0303-114">説明</span><span class="sxs-lookup"><span data-stu-id="d0303-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0303-115">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d0303-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="d0303-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d0303-116">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="d0303-117">危険なユーザーとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d0303-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="d0303-118">RiskyUsers を取得します。</span><span class="sxs-lookup"><span data-stu-id="d0303-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="d0303-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d0303-119">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="d0303-120">特定のリスクの高いユーザーとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="d0303-120">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0303-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0303-121">Properties</span></span>

| <span data-ttu-id="d0303-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0303-122">Property</span></span>   | <span data-ttu-id="d0303-123">型</span><span class="sxs-lookup"><span data-stu-id="d0303-123">Type</span></span>|<span data-ttu-id="d0303-124">説明</span><span class="sxs-lookup"><span data-stu-id="d0303-124">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="d0303-125">リスクのユーザーの一意の id</span><span class="sxs-lookup"><span data-stu-id="d0303-125">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="d0303-126">ユーザーを削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d0303-126">Indicates whether the user is deleted.</span></span> <span data-ttu-id="d0303-127">使用可能な値: `true`、`false`</span><span class="sxs-lookup"><span data-stu-id="d0303-127">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="d0303-128">ユーザーが guest ユーザーであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="d0303-128">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="d0303-129">使用可能な値は、`true`、`false` です。</span><span class="sxs-lookup"><span data-stu-id="d0303-129">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="d0303-130">におけるテナント以外のユーザーの id が存在する場合は true。</span><span class="sxs-lookup"><span data-stu-id="d0303-130">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="d0303-131">このユーザーは、id を使用して、B2B または B2C Azure AD、MSA のまたはサード パーティの id プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="d0303-131">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="d0303-132">におけるテナント内のユーザーの id が存在する場合は false。</span><span class="sxs-lookup"><span data-stu-id="d0303-132">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="d0303-133">危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。</span><span class="sxs-lookup"><span data-stu-id="d0303-133">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="d0303-134">可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d0303-134">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="d0303-135">値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。</span><span class="sxs-lookup"><span data-stu-id="d0303-135">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="d0303-136">危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。</span><span class="sxs-lookup"><span data-stu-id="d0303-136">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="d0303-137">可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d0303-137">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="d0303-138">値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。</span><span class="sxs-lookup"><span data-stu-id="d0303-138">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="d0303-139">危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。</span><span class="sxs-lookup"><span data-stu-id="d0303-139">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="d0303-140">使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d0303-140">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="d0303-141">危険なユーザーが最後に更新されたときの日時</span><span class="sxs-lookup"><span data-stu-id="d0303-141">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="d0303-142">危険なユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="d0303-142">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="d0303-143">危険なユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="d0303-143">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0303-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d0303-144">Relationships</span></span>

| <span data-ttu-id="d0303-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d0303-145">Relationship</span></span> | <span data-ttu-id="d0303-146">型</span><span class="sxs-lookup"><span data-stu-id="d0303-146">Type</span></span> |<span data-ttu-id="d0303-147">説明</span><span class="sxs-lookup"><span data-stu-id="d0303-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0303-148">id</span><span class="sxs-lookup"><span data-stu-id="d0303-148">id</span></span>|<span data-ttu-id="d0303-149">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="d0303-149">UserObjectId</span></span>| <span data-ttu-id="d0303-150">特定のリスク イベントに関連付けられたユーザーの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="d0303-150">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="d0303-151">isGuest</span><span class="sxs-lookup"><span data-stu-id="d0303-151">isGuest</span></span>|<span data-ttu-id="d0303-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="d0303-152">isGuest</span></span>| <span data-ttu-id="d0303-153">危険なユーザーは、ホーム ユーザー (B2E) または (B2B、B2C) は、ゲスト ユーザーのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="d0303-153">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="d0303-154">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d0303-154">isDeleted</span></span>|<span data-ttu-id="d0303-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d0303-155">isDeleted</span></span>| <span data-ttu-id="d0303-156">ユーザーは、可能性があります。 または削除できません。</span><span class="sxs-lookup"><span data-stu-id="d0303-156">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="d0303-157">riskState</span><span class="sxs-lookup"><span data-stu-id="d0303-157">riskState</span></span>|<span data-ttu-id="d0303-158">riskState</span><span class="sxs-lookup"><span data-stu-id="d0303-158">riskState</span></span>| <span data-ttu-id="d0303-159">危険なユーザーは、複数の状態のいずれかに存在でした。</span><span class="sxs-lookup"><span data-stu-id="d0303-159">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="d0303-160">riskDetail</span><span class="sxs-lookup"><span data-stu-id="d0303-160">riskDetail</span></span>|<span data-ttu-id="d0303-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="d0303-161">riskDetail</span></span>| <span data-ttu-id="d0303-162">危険なユーザーは複数の理由により、特定の状態にします。</span><span class="sxs-lookup"><span data-stu-id="d0303-162">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="d0303-163">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d0303-163">riskLevel</span></span>|<span data-ttu-id="d0303-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d0303-164">riskLevel</span></span>| <span data-ttu-id="d0303-165">リスクの高いユーザーと考えられます複数のリスク レベルのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="d0303-165">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d0303-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0303-166">JSON representation</span></span>

<span data-ttu-id="d0303-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d0303-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/riskyuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
