---
title: riskyUsers リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。 この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。
ms.openlocfilehash: 5d51c303d25a781f8e432badb42acb48cf135217
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068300"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="6a756-105">riskyUsers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a756-105">riskyUsers resource type</span></span>

> <span data-ttu-id="6a756-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a756-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a756-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a756-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a756-108">危険にさらされている Azure AD ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="6a756-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="6a756-109">Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。</span><span class="sxs-lookup"><span data-stu-id="6a756-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="6a756-110">この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="6a756-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="6a756-111">リスク イベントの詳細については、 [Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a756-111">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="6a756-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a756-112">Methods</span></span>

| <span data-ttu-id="6a756-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a756-113">Method</span></span>   | <span data-ttu-id="6a756-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6a756-114">Return Type</span></span>|<span data-ttu-id="6a756-115">説明</span><span class="sxs-lookup"><span data-stu-id="6a756-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a756-116">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="6a756-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="6a756-117">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="6a756-117">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="6a756-118">危険なユーザーとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6a756-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="6a756-119">RiskyUsers を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a756-119">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="6a756-120">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="6a756-120">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="6a756-121">特定のリスクの高いユーザーとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="6a756-121">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a756-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a756-122">Properties</span></span>

| <span data-ttu-id="6a756-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a756-123">Property</span></span>   | <span data-ttu-id="6a756-124">型</span><span class="sxs-lookup"><span data-stu-id="6a756-124">Type</span></span>|<span data-ttu-id="6a756-125">説明</span><span class="sxs-lookup"><span data-stu-id="6a756-125">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="6a756-126">リスクのユーザーの一意の id</span><span class="sxs-lookup"><span data-stu-id="6a756-126">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="6a756-127">ユーザーを削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a756-127">Indicates whether the user is deleted.</span></span> <span data-ttu-id="6a756-128">使用可能な値: `true`、`false`</span><span class="sxs-lookup"><span data-stu-id="6a756-128">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="6a756-129">ユーザーが guest ユーザーであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="6a756-129">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="6a756-130">使用可能な値は、`true`、`false` です。</span><span class="sxs-lookup"><span data-stu-id="6a756-130">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="6a756-131">におけるテナント以外のユーザーの id が存在する場合は true。</span><span class="sxs-lookup"><span data-stu-id="6a756-131">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="6a756-132">このユーザーは、id を使用して、B2B または B2C Azure AD、MSA のまたはサード パーティの id プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="6a756-132">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="6a756-133">におけるテナント内のユーザーの id が存在する場合は false。</span><span class="sxs-lookup"><span data-stu-id="6a756-133">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="6a756-134">危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。</span><span class="sxs-lookup"><span data-stu-id="6a756-134">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6a756-135">可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6a756-135">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="6a756-136">値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。</span><span class="sxs-lookup"><span data-stu-id="6a756-136">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="6a756-137">危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。</span><span class="sxs-lookup"><span data-stu-id="6a756-137">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6a756-138">可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6a756-138">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="6a756-139">値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。</span><span class="sxs-lookup"><span data-stu-id="6a756-139">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="6a756-140">危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。</span><span class="sxs-lookup"><span data-stu-id="6a756-140">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="6a756-141">可能な値: `none`、 `confirmedSafe`、 `remediated`、 `dismissed`、 `atRisk`、 `confirmedCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6a756-141">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="6a756-142">危険なユーザーが最後に更新されたときの日時</span><span class="sxs-lookup"><span data-stu-id="6a756-142">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="6a756-143">危険なユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="6a756-143">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="6a756-144">危険なユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="6a756-144">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a756-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a756-145">Relationships</span></span>

| <span data-ttu-id="6a756-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a756-146">Relationship</span></span> | <span data-ttu-id="6a756-147">型</span><span class="sxs-lookup"><span data-stu-id="6a756-147">Type</span></span> |<span data-ttu-id="6a756-148">説明</span><span class="sxs-lookup"><span data-stu-id="6a756-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a756-149">ID</span><span class="sxs-lookup"><span data-stu-id="6a756-149">id</span></span>|<span data-ttu-id="6a756-150">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="6a756-150">UserObjectId</span></span>| <span data-ttu-id="6a756-151">特定のリスク イベントに関連付けられたユーザーの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="6a756-151">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="6a756-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="6a756-152">isGuest</span></span>|<span data-ttu-id="6a756-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="6a756-153">isGuest</span></span>| <span data-ttu-id="6a756-154">危険なユーザーは、ホーム ユーザー (B2E) または (B2B、B2C) は、ゲスト ユーザーのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="6a756-154">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="6a756-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6a756-155">isDeleted</span></span>|<span data-ttu-id="6a756-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6a756-156">isDeleted</span></span>| <span data-ttu-id="6a756-157">ユーザーは、可能性があります。 または削除できません。</span><span class="sxs-lookup"><span data-stu-id="6a756-157">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="6a756-158">riskState</span><span class="sxs-lookup"><span data-stu-id="6a756-158">riskState</span></span>|<span data-ttu-id="6a756-159">riskState</span><span class="sxs-lookup"><span data-stu-id="6a756-159">riskState</span></span>| <span data-ttu-id="6a756-160">危険なユーザーは、複数の状態のいずれかに存在でした。</span><span class="sxs-lookup"><span data-stu-id="6a756-160">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="6a756-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="6a756-161">riskDetail</span></span>|<span data-ttu-id="6a756-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="6a756-162">riskDetail</span></span>| <span data-ttu-id="6a756-163">危険なユーザーは複数の理由により、特定の状態にします。</span><span class="sxs-lookup"><span data-stu-id="6a756-163">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="6a756-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="6a756-164">riskLevel</span></span>|<span data-ttu-id="6a756-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="6a756-165">riskLevel</span></span>| <span data-ttu-id="6a756-166">リスクの高いユーザーと考えられます複数のリスク レベルのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="6a756-166">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6a756-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a756-167">JSON representation</span></span>

<span data-ttu-id="6a756-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a756-168">Here is a JSON representation of the resource.</span></span>

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
"riskState":  {"@odata.type": "microsoft.graph.riskState"}
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
