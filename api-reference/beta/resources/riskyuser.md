---
title: riskyUser リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。 この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 179a6cbddf3e4b27c47761bd81aad1052ae7f728
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343536"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="be6d8-105">riskyUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be6d8-105">riskyUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be6d8-106">危険にさらされている Azure AD ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="be6d8-107">Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="be6d8-108">この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="be6d8-109">リスクイベントの詳細については、「 [Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be6d8-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="be6d8-110">**注:** riskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="be6d8-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="be6d8-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="be6d8-111">Methods</span></span>

| <span data-ttu-id="be6d8-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="be6d8-112">Method</span></span>   | <span data-ttu-id="be6d8-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be6d8-113">Return Type</span></span>|<span data-ttu-id="be6d8-114">説明</span><span class="sxs-lookup"><span data-stu-id="be6d8-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be6d8-115">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="be6d8-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="be6d8-116">[riskyUser](riskyUser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="be6d8-116">[riskyUser](riskyUser.md) collection</span></span>|<span data-ttu-id="be6d8-117">リスクの高いユーザーとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="be6d8-118">riskyUser を取得する</span><span class="sxs-lookup"><span data-stu-id="be6d8-118">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="be6d8-119">riskyUser</span><span class="sxs-lookup"><span data-stu-id="be6d8-119">riskyUser</span></span>](riskyUser.md)|<span data-ttu-id="be6d8-120">特定の危険なユーザーおよびそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="be6d8-121">riskyUsers が侵害されたことを確認する</span><span class="sxs-lookup"><span data-stu-id="be6d8-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="be6d8-122">なし</span><span class="sxs-lookup"><span data-stu-id="be6d8-122">None</span></span> |<span data-ttu-id="be6d8-123">危険なユーザーが侵害されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-123">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="be6d8-124">riskyUsers を閉じる</span><span class="sxs-lookup"><span data-stu-id="be6d8-124">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="be6d8-125">なし</span><span class="sxs-lookup"><span data-stu-id="be6d8-125">None</span></span> | <span data-ttu-id="be6d8-126">危険なユーザーのリスクを無視します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-126">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="be6d8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be6d8-127">Properties</span></span>

| <span data-ttu-id="be6d8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be6d8-128">Property</span></span>   | <span data-ttu-id="be6d8-129">型</span><span class="sxs-lookup"><span data-stu-id="be6d8-129">Type</span></span>|<span data-ttu-id="be6d8-130">説明</span><span class="sxs-lookup"><span data-stu-id="be6d8-130">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="be6d8-131">危険にさらされているユーザーの一意の id</span><span class="sxs-lookup"><span data-stu-id="be6d8-131">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="be6d8-132">ユーザーが削除されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-132">Indicates whether the user is deleted.</span></span> <span data-ttu-id="be6d8-133">可能な値は`true`、です。`false`</span><span class="sxs-lookup"><span data-stu-id="be6d8-133">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="be6d8-134">ユーザーがゲストユーザーであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-134">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="be6d8-135">可能な値は、`true`、`false` です。</span><span class="sxs-lookup"><span data-stu-id="be6d8-135">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="be6d8-136">True の場合は、ユーザーの id がテナントの外部にある場合に考慮します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-136">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="be6d8-137">このユーザーは、Azure AD、MSA、またはサードパーティの id プロバイダーで id を持つ B2B または B2C ユーザーの場合があります。</span><span class="sxs-lookup"><span data-stu-id="be6d8-137">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="be6d8-138">False 場合は、ユーザーの id がテナントの内側にある場合</span><span class="sxs-lookup"><span data-stu-id="be6d8-138">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="be6d8-139">ユーザーの危険な状態がバックエンドによって処理されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="be6d8-139">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="be6d8-140">危険性のあるユーザーが最後に更新された日時</span><span class="sxs-lookup"><span data-stu-id="be6d8-140">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="be6d8-141">使用可能な値は、low、medium、high、hidden、none、unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="be6d8-141">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="be6d8-142">使用可能な値は、none、confirmedSafe、修復済み、atrisk、unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="be6d8-142">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="be6d8-143">使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="be6d8-143">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="be6d8-144">危険ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="be6d8-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="be6d8-145">危険ユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="be6d8-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="be6d8-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be6d8-146">Relationships</span></span>
| <span data-ttu-id="be6d8-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be6d8-147">Relationship</span></span> | <span data-ttu-id="be6d8-148">型</span><span class="sxs-lookup"><span data-stu-id="be6d8-148">Type</span></span>   |<span data-ttu-id="be6d8-149">説明</span><span class="sxs-lookup"><span data-stu-id="be6d8-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be6d8-150">履歴</span><span class="sxs-lookup"><span data-stu-id="be6d8-150">history</span></span>|<span data-ttu-id="be6d8-151">[riskyUserHistoryItem](riskyuserhistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="be6d8-151">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>| |

## <a name="json-representation"></a><span data-ttu-id="be6d8-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be6d8-152">JSON representation</span></span>

<span data-ttu-id="be6d8-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be6d8-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
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
