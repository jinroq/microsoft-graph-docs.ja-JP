---
title: riskyUsers リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。 この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: bb1dab6461a3b235d461720a68855f1e8f3f70d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871555"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="886d3-105">riskyUsers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="886d3-105">riskyUsers resource type</span></span>

> <span data-ttu-id="886d3-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="886d3-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="886d3-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="886d3-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="886d3-108">危険にさらされている Azure AD ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="886d3-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="886d3-109">Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。</span><span class="sxs-lookup"><span data-stu-id="886d3-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="886d3-110">この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="886d3-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="886d3-111">**注:** この API には、Azure AD プレミアム P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="886d3-111">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="886d3-112">リスク イベントの詳細については、 [Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="886d3-112">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="886d3-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="886d3-113">Methods</span></span>

| <span data-ttu-id="886d3-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="886d3-114">Method</span></span>   | <span data-ttu-id="886d3-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="886d3-115">Return Type</span></span>|<span data-ttu-id="886d3-116">説明</span><span class="sxs-lookup"><span data-stu-id="886d3-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="886d3-117">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="886d3-117">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="886d3-118">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="886d3-118">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="886d3-119">危険なユーザーとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="886d3-119">List risky users and their properties.</span></span>|
|[<span data-ttu-id="886d3-120">RiskyUsers を取得します。</span><span class="sxs-lookup"><span data-stu-id="886d3-120">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="886d3-121">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="886d3-121">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="886d3-122">特定のリスクの高いユーザーとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="886d3-122">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="886d3-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="886d3-123">Properties</span></span>

| <span data-ttu-id="886d3-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="886d3-124">Property</span></span>   | <span data-ttu-id="886d3-125">種類</span><span class="sxs-lookup"><span data-stu-id="886d3-125">Type</span></span>|<span data-ttu-id="886d3-126">説明</span><span class="sxs-lookup"><span data-stu-id="886d3-126">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="886d3-127">リスクのユーザーの一意の id</span><span class="sxs-lookup"><span data-stu-id="886d3-127">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="886d3-128">ユーザーを削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="886d3-128">Indicates whether the user is deleted.</span></span> <span data-ttu-id="886d3-129">使用可能な値: `true`、`false`</span><span class="sxs-lookup"><span data-stu-id="886d3-129">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="886d3-130">ユーザーが guest ユーザーであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="886d3-130">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="886d3-131">使用可能な値は、`true`、`false` です。</span><span class="sxs-lookup"><span data-stu-id="886d3-131">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="886d3-132">におけるテナント以外のユーザーの id が存在する場合は true。</span><span class="sxs-lookup"><span data-stu-id="886d3-132">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="886d3-133">このユーザーは、id を使用して、B2B または B2C Azure AD、MSA のまたはサード パーティの id プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="886d3-133">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="886d3-134">におけるテナント内のユーザーの id が存在する場合は false。</span><span class="sxs-lookup"><span data-stu-id="886d3-134">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="886d3-135">危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。</span><span class="sxs-lookup"><span data-stu-id="886d3-135">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="886d3-136">可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="886d3-136">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="886d3-137">値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。</span><span class="sxs-lookup"><span data-stu-id="886d3-137">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="886d3-138">危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。</span><span class="sxs-lookup"><span data-stu-id="886d3-138">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="886d3-139">可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="886d3-139">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="886d3-140">値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。</span><span class="sxs-lookup"><span data-stu-id="886d3-140">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="886d3-141">危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。</span><span class="sxs-lookup"><span data-stu-id="886d3-141">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="886d3-142">可能な値: `none`、 `confirmedSafe`、 `remediated`、 `dismissed`、 `atRisk`、 `confirmedCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="886d3-142">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="886d3-143">危険なユーザーが最後に更新されたときの日時</span><span class="sxs-lookup"><span data-stu-id="886d3-143">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="886d3-144">危険なユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="886d3-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="886d3-145">危険なユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="886d3-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="886d3-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="886d3-146">Relationships</span></span>

| <span data-ttu-id="886d3-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="886d3-147">Relationship</span></span> | <span data-ttu-id="886d3-148">型</span><span class="sxs-lookup"><span data-stu-id="886d3-148">Type</span></span> |<span data-ttu-id="886d3-149">説明</span><span class="sxs-lookup"><span data-stu-id="886d3-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="886d3-150">ID</span><span class="sxs-lookup"><span data-stu-id="886d3-150">id</span></span>|<span data-ttu-id="886d3-151">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="886d3-151">UserObjectId</span></span>| <span data-ttu-id="886d3-152">特定のリスク イベントに関連付けられたユーザーの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="886d3-152">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="886d3-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="886d3-153">isGuest</span></span>|<span data-ttu-id="886d3-154">isGuest</span><span class="sxs-lookup"><span data-stu-id="886d3-154">isGuest</span></span>| <span data-ttu-id="886d3-155">危険なユーザーは、ホーム ユーザー (B2E) または (B2B、B2C) は、ゲスト ユーザーのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="886d3-155">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="886d3-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="886d3-156">isDeleted</span></span>|<span data-ttu-id="886d3-157">isDeleted</span><span class="sxs-lookup"><span data-stu-id="886d3-157">isDeleted</span></span>| <span data-ttu-id="886d3-158">ユーザーは、可能性があります。 または削除できません。</span><span class="sxs-lookup"><span data-stu-id="886d3-158">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="886d3-159">riskState</span><span class="sxs-lookup"><span data-stu-id="886d3-159">riskState</span></span>|<span data-ttu-id="886d3-160">riskState</span><span class="sxs-lookup"><span data-stu-id="886d3-160">riskState</span></span>| <span data-ttu-id="886d3-161">危険なユーザーは、複数の状態のいずれかに存在でした。</span><span class="sxs-lookup"><span data-stu-id="886d3-161">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="886d3-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="886d3-162">riskDetail</span></span>|<span data-ttu-id="886d3-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="886d3-163">riskDetail</span></span>| <span data-ttu-id="886d3-164">危険なユーザーは複数の理由により、特定の状態にします。</span><span class="sxs-lookup"><span data-stu-id="886d3-164">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="886d3-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="886d3-165">riskLevel</span></span>|<span data-ttu-id="886d3-166">riskLevel</span><span class="sxs-lookup"><span data-stu-id="886d3-166">riskLevel</span></span>| <span data-ttu-id="886d3-167">リスクの高いユーザーと考えられます複数のリスク レベルのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="886d3-167">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="886d3-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="886d3-168">JSON representation</span></span>

<span data-ttu-id="886d3-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="886d3-169">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
