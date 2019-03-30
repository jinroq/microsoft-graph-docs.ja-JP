---
title: riskyUsers リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。 この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003721"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="9c2ee-105">riskyUsers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c2ee-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c2ee-106">危険にさらされている Azure AD ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="9c2ee-107">Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="9c2ee-108">この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="9c2ee-109">リスクイベントの詳細については、「 [Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="9c2ee-110">**注:** riskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="9c2ee-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c2ee-111">Methods</span></span>

| <span data-ttu-id="9c2ee-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c2ee-112">Method</span></span>   | <span data-ttu-id="9c2ee-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9c2ee-113">Return Type</span></span>|<span data-ttu-id="9c2ee-114">説明</span><span class="sxs-lookup"><span data-stu-id="9c2ee-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c2ee-115">リスト riskyUsers</span><span class="sxs-lookup"><span data-stu-id="9c2ee-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="9c2ee-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="9c2ee-116">riskyUsers</span></span>](riskyUser.md) |<span data-ttu-id="9c2ee-117">リスクの高いユーザーとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="9c2ee-118">riskyUsers を取得する</span><span class="sxs-lookup"><span data-stu-id="9c2ee-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="9c2ee-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="9c2ee-119">riskyUsers</span></span>](riskyUser.md)|<span data-ttu-id="9c2ee-120">特定の危険なユーザーおよびそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="9c2ee-121">riskyUsers が侵害されたことを確認する</span><span class="sxs-lookup"><span data-stu-id="9c2ee-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="9c2ee-122">危険なユーザーが侵害されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-122">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="9c2ee-123">riskyUsers を閉じる</span><span class="sxs-lookup"><span data-stu-id="9c2ee-123">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="9c2ee-124">危険なユーザーのリスクを無視します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-124">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c2ee-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c2ee-125">Properties</span></span>

| <span data-ttu-id="9c2ee-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c2ee-126">Property</span></span>   | <span data-ttu-id="9c2ee-127">型</span><span class="sxs-lookup"><span data-stu-id="9c2ee-127">Type</span></span>|<span data-ttu-id="9c2ee-128">説明</span><span class="sxs-lookup"><span data-stu-id="9c2ee-128">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="9c2ee-129">危険にさらされているユーザーの一意の id</span><span class="sxs-lookup"><span data-stu-id="9c2ee-129">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="9c2ee-130">ユーザーが削除されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-130">Indicates whether the user is deleted.</span></span> <span data-ttu-id="9c2ee-131">可能な値は`true`、です。`false`</span><span class="sxs-lookup"><span data-stu-id="9c2ee-131">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="9c2ee-132">ユーザーがゲストユーザーであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-132">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="9c2ee-133">可能な値は、`true`、`false` です。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-133">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="9c2ee-134">True の場合は、ユーザーの id がテナントの外部にある場合に考慮します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-134">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="9c2ee-135">このユーザーは、Azure AD、MSA、またはサードパーティの id プロバイダーで id を持つ B2B または B2C ユーザーの場合があります。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-135">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="9c2ee-136">False 場合は、ユーザーの id がテナントの内側にある場合</span><span class="sxs-lookup"><span data-stu-id="9c2ee-136">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="9c2ee-137">ユーザーの危険な状態がバックエンドによって処理されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-137">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`risk`|[<span data-ttu-id="9c2ee-138">さらさ</span><span class="sxs-lookup"><span data-stu-id="9c2ee-138">risk</span></span>](risk.md)|<span data-ttu-id="9c2ee-139">危険ユーザーの状態</span><span class="sxs-lookup"><span data-stu-id="9c2ee-139">Risky user state</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="9c2ee-140">危険性のあるユーザーが最後に更新された日時</span><span class="sxs-lookup"><span data-stu-id="9c2ee-140">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="9c2ee-141">危険ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="9c2ee-141">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="9c2ee-142">危険ユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="9c2ee-142">Risky user principal name</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9c2ee-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c2ee-143">JSON representation</span></span>

<span data-ttu-id="9c2ee-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9c2ee-144">Here is a JSON representation of the resource.</span></span>

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
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
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
