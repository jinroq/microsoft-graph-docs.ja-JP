---
title: riskyUser リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。 この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3548be0439eaa5335d710a35f51fdbaecb19060c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008727"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="68d77-105">riskyUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68d77-105">riskyUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68d77-106">危険にさらされている Azure AD ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="68d77-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="68d77-107">Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。</span><span class="sxs-lookup"><span data-stu-id="68d77-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="68d77-108">この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="68d77-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="68d77-109">リスクイベントの詳細については、「 [Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68d77-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="68d77-110">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="68d77-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="68d77-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="68d77-111">Methods</span></span>

| <span data-ttu-id="68d77-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="68d77-112">Method</span></span>   | <span data-ttu-id="68d77-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="68d77-113">Return Type</span></span>|<span data-ttu-id="68d77-114">説明</span><span class="sxs-lookup"><span data-stu-id="68d77-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68d77-115">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="68d77-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="68d77-116">[riskyUser](riskyuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="68d77-116">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="68d77-117">リスクの高いユーザーとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="68d77-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="68d77-118">RiskyUser を取得する</span><span class="sxs-lookup"><span data-stu-id="68d77-118">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="68d77-119">riskyUser</span><span class="sxs-lookup"><span data-stu-id="68d77-119">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="68d77-120">特定の危険なユーザーおよびそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="68d77-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="68d77-121">リストの履歴</span><span class="sxs-lookup"><span data-stu-id="68d77-121">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="68d77-122">[riskyUserHistoryItem](riskyuserhistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="68d77-122">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="68d77-123">Azure AD ユーザーのリスク履歴を取得します。</span><span class="sxs-lookup"><span data-stu-id="68d77-123">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="68d77-124">RiskyUsers が侵害されたことを確認する</span><span class="sxs-lookup"><span data-stu-id="68d77-124">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="68d77-125">None</span><span class="sxs-lookup"><span data-stu-id="68d77-125">None</span></span> |<span data-ttu-id="68d77-126">危険なユーザーが侵害されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="68d77-126">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="68d77-127">RiskyUsers を閉じる</span><span class="sxs-lookup"><span data-stu-id="68d77-127">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="68d77-128">None</span><span class="sxs-lookup"><span data-stu-id="68d77-128">None</span></span> | <span data-ttu-id="68d77-129">危険なユーザーのリスクを無視します。</span><span class="sxs-lookup"><span data-stu-id="68d77-129">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="68d77-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68d77-130">Properties</span></span>

| <span data-ttu-id="68d77-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68d77-131">Property</span></span>   | <span data-ttu-id="68d77-132">型</span><span class="sxs-lookup"><span data-stu-id="68d77-132">Type</span></span>|<span data-ttu-id="68d77-133">説明</span><span class="sxs-lookup"><span data-stu-id="68d77-133">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="68d77-134">危険にさらされているユーザーの一意の id</span><span class="sxs-lookup"><span data-stu-id="68d77-134">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="68d77-135">ユーザーが削除されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="68d77-135">Indicates whether the user is deleted.</span></span> <span data-ttu-id="68d77-136">可能な値は`true`、です。`false`</span><span class="sxs-lookup"><span data-stu-id="68d77-136">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="68d77-137">ユーザーがゲストユーザーであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="68d77-137">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="68d77-138">可能な値は、`true`、`false` です。</span><span class="sxs-lookup"><span data-stu-id="68d77-138">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="68d77-139">True の場合は、ユーザーの id がテナントの外部にある場合に考慮します。</span><span class="sxs-lookup"><span data-stu-id="68d77-139">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="68d77-140">このユーザーは、Azure AD、MSA、またはサードパーティの id プロバイダーで id を持つ B2B または B2C ユーザーの場合があります。</span><span class="sxs-lookup"><span data-stu-id="68d77-140">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="68d77-141">False 場合は、ユーザーの id がテナントの内側にある場合</span><span class="sxs-lookup"><span data-stu-id="68d77-141">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="68d77-142">ユーザーの危険な状態がバックエンドによって処理されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="68d77-142">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="68d77-143">危険性のあるユーザーが最後に更新された日時</span><span class="sxs-lookup"><span data-stu-id="68d77-143">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="68d77-144">使用可能な値は、low、medium、high、hidden、none、Unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="68d77-144">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="68d77-145">使用可能な値は、none、confirmedSafe、修復済み、atRisk、Unknownfuturevalue というです。</span><span class="sxs-lookup"><span data-stu-id="68d77-145">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="68d77-146">使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、Unknownfuturevalue という。</span><span class="sxs-lookup"><span data-stu-id="68d77-146">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="68d77-147">危険ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="68d77-147">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="68d77-148">危険ユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="68d77-148">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="68d77-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68d77-149">Relationships</span></span>
| <span data-ttu-id="68d77-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68d77-150">Relationship</span></span> | <span data-ttu-id="68d77-151">型</span><span class="sxs-lookup"><span data-stu-id="68d77-151">Type</span></span>   |<span data-ttu-id="68d77-152">説明</span><span class="sxs-lookup"><span data-stu-id="68d77-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68d77-153">履歴</span><span class="sxs-lookup"><span data-stu-id="68d77-153">history</span></span>|<span data-ttu-id="68d77-154">[riskyUserHistoryItem](riskyuserhistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="68d77-154">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="68d77-155">Azure ad Id 保護によって決定された Azure AD ユーザーのリスク履歴を表します。</span><span class="sxs-lookup"><span data-stu-id="68d77-155">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68d77-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68d77-156">JSON representation</span></span>

<span data-ttu-id="68d77-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68d77-157">Here is a JSON representation of the resource.</span></span>

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
