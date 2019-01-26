---
title: riskyUsers リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。 この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 875df6db36e4075d0d02a682ede5c177d49cfe7d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572186"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="b311f-105">riskyUsers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b311f-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b311f-106">危険にさらされている Azure AD ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="b311f-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="b311f-107">Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。</span><span class="sxs-lookup"><span data-stu-id="b311f-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="b311f-108">この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="b311f-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="b311f-109">**注:** この API には、Azure AD プレミアム P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b311f-109">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="b311f-110">リスク イベントの詳細については、 [Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b311f-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="b311f-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="b311f-111">Methods</span></span>

| <span data-ttu-id="b311f-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="b311f-112">Method</span></span>   | <span data-ttu-id="b311f-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b311f-113">Return Type</span></span>|<span data-ttu-id="b311f-114">説明</span><span class="sxs-lookup"><span data-stu-id="b311f-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b311f-115">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b311f-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="b311f-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b311f-116">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="b311f-117">危険なユーザーとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b311f-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="b311f-118">RiskyUsers を取得します。</span><span class="sxs-lookup"><span data-stu-id="b311f-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="b311f-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b311f-119">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="b311f-120">特定のリスクの高いユーザーとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="b311f-120">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="b311f-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b311f-121">Properties</span></span>

| <span data-ttu-id="b311f-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b311f-122">Property</span></span>   | <span data-ttu-id="b311f-123">型</span><span class="sxs-lookup"><span data-stu-id="b311f-123">Type</span></span>|<span data-ttu-id="b311f-124">説明</span><span class="sxs-lookup"><span data-stu-id="b311f-124">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="b311f-125">リスクのユーザーの一意の id</span><span class="sxs-lookup"><span data-stu-id="b311f-125">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="b311f-126">ユーザーを削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b311f-126">Indicates whether the user is deleted.</span></span> <span data-ttu-id="b311f-127">使用可能な値: `true`、`false`</span><span class="sxs-lookup"><span data-stu-id="b311f-127">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="b311f-128">ユーザーが guest ユーザーであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="b311f-128">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="b311f-129">使用可能な値は、`true`、`false` です。</span><span class="sxs-lookup"><span data-stu-id="b311f-129">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="b311f-130">におけるテナント以外のユーザーの id が存在する場合は true。</span><span class="sxs-lookup"><span data-stu-id="b311f-130">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="b311f-131">このユーザーは、id を使用して、B2B または B2C Azure AD、MSA のまたはサード パーティの id プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="b311f-131">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="b311f-132">におけるテナント内のユーザーの id が存在する場合は false。</span><span class="sxs-lookup"><span data-stu-id="b311f-132">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="b311f-133">危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。</span><span class="sxs-lookup"><span data-stu-id="b311f-133">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b311f-134">可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b311f-134">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="b311f-135">値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。</span><span class="sxs-lookup"><span data-stu-id="b311f-135">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="b311f-136">危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。</span><span class="sxs-lookup"><span data-stu-id="b311f-136">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b311f-137">可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b311f-137">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="b311f-138">値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。</span><span class="sxs-lookup"><span data-stu-id="b311f-138">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="b311f-139">危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。</span><span class="sxs-lookup"><span data-stu-id="b311f-139">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b311f-140">使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b311f-140">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="b311f-141">危険なユーザーが最後に更新されたときの日時</span><span class="sxs-lookup"><span data-stu-id="b311f-141">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="b311f-142">危険なユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="b311f-142">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="b311f-143">危険なユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="b311f-143">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="b311f-144">関係</span><span class="sxs-lookup"><span data-stu-id="b311f-144">Relationships</span></span>

| <span data-ttu-id="b311f-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b311f-145">Relationship</span></span> | <span data-ttu-id="b311f-146">型</span><span class="sxs-lookup"><span data-stu-id="b311f-146">Type</span></span> |<span data-ttu-id="b311f-147">説明</span><span class="sxs-lookup"><span data-stu-id="b311f-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b311f-148">id</span><span class="sxs-lookup"><span data-stu-id="b311f-148">id</span></span>|<span data-ttu-id="b311f-149">文字列</span><span class="sxs-lookup"><span data-stu-id="b311f-149">string</span></span>| <span data-ttu-id="b311f-150">特定のリスク イベントに関連付けられたユーザーの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="b311f-150">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="b311f-151">isGuest</span><span class="sxs-lookup"><span data-stu-id="b311f-151">isGuest</span></span>|<span data-ttu-id="b311f-152">boolean</span><span class="sxs-lookup"><span data-stu-id="b311f-152">boolean</span></span>| <span data-ttu-id="b311f-153">危険なユーザーは、ホーム ユーザー (B2E) または (B2B、B2C) は、ゲスト ユーザーのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="b311f-153">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="b311f-154">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b311f-154">isDeleted</span></span>|<span data-ttu-id="b311f-155">boolean</span><span class="sxs-lookup"><span data-stu-id="b311f-155">boolean</span></span>| <span data-ttu-id="b311f-156">ユーザーは、可能性があります。 または削除できません。</span><span class="sxs-lookup"><span data-stu-id="b311f-156">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="b311f-157">riskState</span><span class="sxs-lookup"><span data-stu-id="b311f-157">riskState</span></span>|<span data-ttu-id="b311f-158">riskState</span><span class="sxs-lookup"><span data-stu-id="b311f-158">riskState</span></span>| <span data-ttu-id="b311f-159">危険なユーザーは、複数の状態のいずれかに存在でした。</span><span class="sxs-lookup"><span data-stu-id="b311f-159">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="b311f-160">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b311f-160">riskDetail</span></span>|<span data-ttu-id="b311f-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b311f-161">riskDetail</span></span>| <span data-ttu-id="b311f-162">危険なユーザーは複数の理由により、特定の状態にします。</span><span class="sxs-lookup"><span data-stu-id="b311f-162">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="b311f-163">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b311f-163">riskLevel</span></span>|<span data-ttu-id="b311f-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b311f-164">riskLevel</span></span>| <span data-ttu-id="b311f-165">リスクの高いユーザーと考えられます複数のリスク レベルのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="b311f-165">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b311f-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b311f-166">JSON representation</span></span>

<span data-ttu-id="b311f-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b311f-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.riskyUser"
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
