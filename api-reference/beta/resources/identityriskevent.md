---
title: identityRiskEvent リソースの種類
description: Azure Active Directory アイデンティティ保護によって検出されたリスク イベントです。 特定のリスク イベントの種類ごとの基本型です。
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: 0735599c260fac178b54ee4ba54a17f5ea027e23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858997"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="21b62-104">identityRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21b62-104">identityRiskEvent resource type</span></span>

> <span data-ttu-id="21b62-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="21b62-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21b62-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21b62-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21b62-107">[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="21b62-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="21b62-108">特定のリスク イベントの種類ごとの基本型です。</span><span class="sxs-lookup"><span data-stu-id="21b62-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="21b62-109">イベントの種類</span><span class="sxs-lookup"><span data-stu-id="21b62-109">Event type</span></span>         | <span data-ttu-id="21b62-110">説明</span><span class="sxs-lookup"><span data-stu-id="21b62-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="21b62-111">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="21b62-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="21b62-112">匿名の IP アドレスからサインインの問題です。</span><span class="sxs-lookup"><span data-stu-id="21b62-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="21b62-113">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="21b62-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="21b62-114">サインインがマルウェアに感染したデバイスから。</span><span class="sxs-lookup"><span data-stu-id="21b62-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="21b62-115">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="21b62-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="21b62-116">典型的な場所に旅行を不可能になります。</span><span class="sxs-lookup"><span data-stu-id="21b62-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="21b62-117">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="21b62-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="21b62-118">リークした資格情報を持つユーザーです。</span><span class="sxs-lookup"><span data-stu-id="21b62-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="21b62-119">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="21b62-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="21b62-120">不審な IP アドレスからサインインの問題です。</span><span class="sxs-lookup"><span data-stu-id="21b62-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="21b62-121">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="21b62-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="21b62-122">未知の場所からサインインの問題です。</span><span class="sxs-lookup"><span data-stu-id="21b62-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="21b62-123">リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="21b62-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="21b62-124">メソッド</span><span class="sxs-lookup"><span data-stu-id="21b62-124">Methods</span></span>

| <span data-ttu-id="21b62-125">メソッド</span><span class="sxs-lookup"><span data-stu-id="21b62-125">Method</span></span>           | <span data-ttu-id="21b62-126">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="21b62-126">Return Type</span></span>    |<span data-ttu-id="21b62-127">説明</span><span class="sxs-lookup"><span data-stu-id="21b62-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21b62-128">IdentityRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="21b62-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="21b62-129">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="21b62-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="21b62-130">IdentityRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21b62-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21b62-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21b62-131">Properties</span></span>
| <span data-ttu-id="21b62-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21b62-132">Property</span></span>     | <span data-ttu-id="21b62-133">種類</span><span class="sxs-lookup"><span data-stu-id="21b62-133">Type</span></span>   |<span data-ttu-id="21b62-134">説明</span><span class="sxs-lookup"><span data-stu-id="21b62-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21b62-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="21b62-135">closedDateTime</span></span>|<span data-ttu-id="21b62-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b62-136">dateTimeOffset</span></span>| <span data-ttu-id="21b62-137">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="21b62-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="21b62-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21b62-138">createdDateTime</span></span>|<span data-ttu-id="21b62-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b62-139">dateTimeOffset</span></span>| <span data-ttu-id="21b62-140">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="21b62-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="21b62-141">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="21b62-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="21b62-142">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="21b62-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="21b62-143">ID</span><span class="sxs-lookup"><span data-stu-id="21b62-143">id</span></span>|<span data-ttu-id="21b62-144">文字列</span><span class="sxs-lookup"><span data-stu-id="21b62-144">string</span></span>| <span data-ttu-id="21b62-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21b62-145">Read-only</span></span>|
|<span data-ttu-id="21b62-146">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="21b62-146">riskEventDateTime</span></span>|<span data-ttu-id="21b62-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b62-147">dateTimeOffset</span></span>| <span data-ttu-id="21b62-148">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="21b62-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="21b62-149">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="21b62-149">riskEventStatus</span></span>|<span data-ttu-id="21b62-150">文字列</span><span class="sxs-lookup"><span data-stu-id="21b62-150">string</span></span>| <span data-ttu-id="21b62-151">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="21b62-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="21b62-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="21b62-152">riskLevel</span></span>|<span data-ttu-id="21b62-153">文字列</span><span class="sxs-lookup"><span data-stu-id="21b62-153">string</span></span>| <span data-ttu-id="21b62-154">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="21b62-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="21b62-155">riskEventType</span><span class="sxs-lookup"><span data-stu-id="21b62-155">riskEventType</span></span>|<span data-ttu-id="21b62-156">文字列</span><span class="sxs-lookup"><span data-stu-id="21b62-156">string</span></span>| <span data-ttu-id="21b62-157">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="21b62-157">The type of risk</span></span>|
|<span data-ttu-id="21b62-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="21b62-158">userDisplayName</span></span>|<span data-ttu-id="21b62-159">文字列</span><span class="sxs-lookup"><span data-stu-id="21b62-159">string</span></span>| <span data-ttu-id="21b62-160">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="21b62-160">The name of the user at risk</span></span>|
|<span data-ttu-id="21b62-161">userId</span><span class="sxs-lookup"><span data-stu-id="21b62-161">userId</span></span>|<span data-ttu-id="21b62-162">文字列</span><span class="sxs-lookup"><span data-stu-id="21b62-162">string</span></span>| <span data-ttu-id="21b62-163">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="21b62-163">The id of the user at risk</span></span>|
|<span data-ttu-id="21b62-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21b62-164">userPrincipalName</span></span>|<span data-ttu-id="21b62-165">文字列</span><span class="sxs-lookup"><span data-stu-id="21b62-165">string</span></span>| <span data-ttu-id="21b62-166">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="21b62-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="21b62-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21b62-167">Relationships</span></span>
| <span data-ttu-id="21b62-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21b62-168">Relationship</span></span> | <span data-ttu-id="21b62-169">型</span><span class="sxs-lookup"><span data-stu-id="21b62-169">Type</span></span>   |<span data-ttu-id="21b62-170">説明</span><span class="sxs-lookup"><span data-stu-id="21b62-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21b62-171">impactedUser</span><span class="sxs-lookup"><span data-stu-id="21b62-171">impactedUser</span></span>|[<span data-ttu-id="21b62-172">user</span><span class="sxs-lookup"><span data-stu-id="21b62-172">user</span></span>](user.md)| <span data-ttu-id="21b62-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="21b62-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21b62-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21b62-175">JSON representation</span></span>

<span data-ttu-id="21b62-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21b62-176">Here is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
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
