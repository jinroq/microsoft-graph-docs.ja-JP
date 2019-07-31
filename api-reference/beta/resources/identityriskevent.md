---
title: identityRiskEvent リソースの種類
description: Azure Active Directory Id 保護によって検出されたリスクイベント。 これは、各固有のリスクイベントの種類の基本型です。
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7ea0a11931021e828660cc7b03991b8ea96ef1f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005801"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="e56c5-104">identityRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e56c5-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e56c5-105">[Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスクイベント。</span><span class="sxs-lookup"><span data-stu-id="e56c5-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="e56c5-106">これは、各固有のリスクイベントの種類の基本型です。</span><span class="sxs-lookup"><span data-stu-id="e56c5-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="e56c5-107">イベントの種類</span><span class="sxs-lookup"><span data-stu-id="e56c5-107">Event type</span></span>         | <span data-ttu-id="e56c5-108">説明</span><span class="sxs-lookup"><span data-stu-id="e56c5-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="e56c5-109">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e56c5-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="e56c5-110">匿名 IP アドレスからのサインイン。</span><span class="sxs-lookup"><span data-stu-id="e56c5-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="e56c5-111">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e56c5-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="e56c5-112">マルウェアに感染したデバイスからのサインイン。</span><span class="sxs-lookup"><span data-stu-id="e56c5-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="e56c5-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e56c5-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="e56c5-114">例外的でない場所への移動は不可能です。</span><span class="sxs-lookup"><span data-stu-id="e56c5-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="e56c5-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e56c5-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="e56c5-116">資格情報がリークしたユーザー。</span><span class="sxs-lookup"><span data-stu-id="e56c5-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="e56c5-117">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e56c5-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="e56c5-118">疑わしい IP アドレスからのサインイン。</span><span class="sxs-lookup"><span data-stu-id="e56c5-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="e56c5-119">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e56c5-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="e56c5-120">見慣れない場所からのサインイン。</span><span class="sxs-lookup"><span data-stu-id="e56c5-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="e56c5-121">リスクイベントに関する詳細な情報については、「 [AZURE AD Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)」のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e56c5-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="e56c5-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="e56c5-122">Methods</span></span>

| <span data-ttu-id="e56c5-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="e56c5-123">Method</span></span>           | <span data-ttu-id="e56c5-124">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e56c5-124">Return Type</span></span>    |<span data-ttu-id="e56c5-125">説明</span><span class="sxs-lookup"><span data-stu-id="e56c5-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e56c5-126">identityRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="e56c5-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="e56c5-127">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e56c5-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="e56c5-128">IdentityRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e56c5-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e56c5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e56c5-129">Properties</span></span>
| <span data-ttu-id="e56c5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e56c5-130">Property</span></span>     | <span data-ttu-id="e56c5-131">型</span><span class="sxs-lookup"><span data-stu-id="e56c5-131">Type</span></span>   |<span data-ttu-id="e56c5-132">説明</span><span class="sxs-lookup"><span data-stu-id="e56c5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e56c5-133">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e56c5-133">closedDateTime</span></span>|<span data-ttu-id="e56c5-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e56c5-134">dateTimeOffset</span></span>| <span data-ttu-id="e56c5-135">リスクイベントが終了した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="e56c5-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e56c5-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e56c5-136">createdDateTime</span></span>|<span data-ttu-id="e56c5-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e56c5-137">dateTimeOffset</span></span>| <span data-ttu-id="e56c5-138">リスクイベントが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e56c5-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="e56c5-139">これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。</span><span class="sxs-lookup"><span data-stu-id="e56c5-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e56c5-140">これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="e56c5-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e56c5-141">id</span><span class="sxs-lookup"><span data-stu-id="e56c5-141">id</span></span>|<span data-ttu-id="e56c5-142">string</span><span class="sxs-lookup"><span data-stu-id="e56c5-142">string</span></span>| <span data-ttu-id="e56c5-143">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="e56c5-143">Read-only</span></span>|
|<span data-ttu-id="e56c5-144">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="e56c5-144">riskEventDateTime</span></span>|<span data-ttu-id="e56c5-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e56c5-145">dateTimeOffset</span></span>| <span data-ttu-id="e56c5-146">リスクイベントが発生した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="e56c5-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="e56c5-147">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="e56c5-147">riskEventStatus</span></span>|<span data-ttu-id="e56c5-148">string</span><span class="sxs-lookup"><span data-stu-id="e56c5-148">string</span></span>| <span data-ttu-id="e56c5-149">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="e56c5-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e56c5-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e56c5-150">riskLevel</span></span>|<span data-ttu-id="e56c5-151">string</span><span class="sxs-lookup"><span data-stu-id="e56c5-151">string</span></span>| <span data-ttu-id="e56c5-152">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e56c5-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e56c5-153">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e56c5-153">riskEventType</span></span>|<span data-ttu-id="e56c5-154">string</span><span class="sxs-lookup"><span data-stu-id="e56c5-154">string</span></span>| <span data-ttu-id="e56c5-155">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="e56c5-155">The type of risk</span></span>|
|<span data-ttu-id="e56c5-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e56c5-156">userDisplayName</span></span>|<span data-ttu-id="e56c5-157">string</span><span class="sxs-lookup"><span data-stu-id="e56c5-157">string</span></span>| <span data-ttu-id="e56c5-158">リスクのあるユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="e56c5-158">The name of the user at risk</span></span>|
|<span data-ttu-id="e56c5-159">userId</span><span class="sxs-lookup"><span data-stu-id="e56c5-159">userId</span></span>|<span data-ttu-id="e56c5-160">string</span><span class="sxs-lookup"><span data-stu-id="e56c5-160">string</span></span>| <span data-ttu-id="e56c5-161">リスクがあるユーザーの id</span><span class="sxs-lookup"><span data-stu-id="e56c5-161">The id of the user at risk</span></span>|
|<span data-ttu-id="e56c5-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e56c5-162">userPrincipalName</span></span>|<span data-ttu-id="e56c5-163">string</span><span class="sxs-lookup"><span data-stu-id="e56c5-163">string</span></span>| <span data-ttu-id="e56c5-164">リスクがあるユーザーのユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="e56c5-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e56c5-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e56c5-165">Relationships</span></span>
| <span data-ttu-id="e56c5-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e56c5-166">Relationship</span></span> | <span data-ttu-id="e56c5-167">型</span><span class="sxs-lookup"><span data-stu-id="e56c5-167">Type</span></span>   |<span data-ttu-id="e56c5-168">説明</span><span class="sxs-lookup"><span data-stu-id="e56c5-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e56c5-169">impactedUser</span><span class="sxs-lookup"><span data-stu-id="e56c5-169">impactedUser</span></span>|[<span data-ttu-id="e56c5-170">ユーザー</span><span class="sxs-lookup"><span data-stu-id="e56c5-170">user</span></span>](user.md)| <span data-ttu-id="e56c5-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="e56c5-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e56c5-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e56c5-173">JSON representation</span></span>

<span data-ttu-id="e56c5-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e56c5-174">Here is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
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
  "suppressions": []
}
-->
