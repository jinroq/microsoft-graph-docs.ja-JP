---
title: identityRiskEvent リソースの種類
description: Azure Active Directory アイデンティティ保護によって検出されたリスク イベントです。 特定のリスク イベントの種類ごとの基本型です。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514181"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="f02a8-104">identityRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f02a8-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f02a8-105">[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="f02a8-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="f02a8-106">特定のリスク イベントの種類ごとの基本型です。</span><span class="sxs-lookup"><span data-stu-id="f02a8-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="f02a8-107">イベントの種類</span><span class="sxs-lookup"><span data-stu-id="f02a8-107">Event type</span></span>         | <span data-ttu-id="f02a8-108">説明</span><span class="sxs-lookup"><span data-stu-id="f02a8-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="f02a8-109">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f02a8-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="f02a8-110">匿名の IP アドレスからサインインの問題です。</span><span class="sxs-lookup"><span data-stu-id="f02a8-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="f02a8-111">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f02a8-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="f02a8-112">サインインがマルウェアに感染したデバイスから。</span><span class="sxs-lookup"><span data-stu-id="f02a8-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="f02a8-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f02a8-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="f02a8-114">典型的な場所に旅行を不可能になります。</span><span class="sxs-lookup"><span data-stu-id="f02a8-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="f02a8-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f02a8-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="f02a8-116">リークした資格情報を持つユーザーです。</span><span class="sxs-lookup"><span data-stu-id="f02a8-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="f02a8-117">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f02a8-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="f02a8-118">不審な IP アドレスからサインインの問題です。</span><span class="sxs-lookup"><span data-stu-id="f02a8-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="f02a8-119">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f02a8-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="f02a8-120">未知の場所からサインインの問題です。</span><span class="sxs-lookup"><span data-stu-id="f02a8-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="f02a8-121">リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="f02a8-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="f02a8-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="f02a8-122">Methods</span></span>

| <span data-ttu-id="f02a8-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="f02a8-123">Method</span></span>           | <span data-ttu-id="f02a8-124">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f02a8-124">Return Type</span></span>    |<span data-ttu-id="f02a8-125">説明</span><span class="sxs-lookup"><span data-stu-id="f02a8-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f02a8-126">IdentityRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="f02a8-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="f02a8-127">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f02a8-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="f02a8-128">IdentityRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f02a8-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f02a8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f02a8-129">Properties</span></span>
| <span data-ttu-id="f02a8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f02a8-130">Property</span></span>     | <span data-ttu-id="f02a8-131">型</span><span class="sxs-lookup"><span data-stu-id="f02a8-131">Type</span></span>   |<span data-ttu-id="f02a8-132">説明</span><span class="sxs-lookup"><span data-stu-id="f02a8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f02a8-133">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f02a8-133">closedDateTime</span></span>|<span data-ttu-id="f02a8-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f02a8-134">dateTimeOffset</span></span>| <span data-ttu-id="f02a8-135">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="f02a8-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f02a8-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f02a8-136">createdDateTime</span></span>|<span data-ttu-id="f02a8-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f02a8-137">dateTimeOffset</span></span>| <span data-ttu-id="f02a8-138">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="f02a8-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="f02a8-139">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="f02a8-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f02a8-140">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="f02a8-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f02a8-141">id</span><span class="sxs-lookup"><span data-stu-id="f02a8-141">id</span></span>|<span data-ttu-id="f02a8-142">string</span><span class="sxs-lookup"><span data-stu-id="f02a8-142">string</span></span>| <span data-ttu-id="f02a8-143">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="f02a8-143">Read-only</span></span>|
|<span data-ttu-id="f02a8-144">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="f02a8-144">riskEventDateTime</span></span>|<span data-ttu-id="f02a8-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f02a8-145">dateTimeOffset</span></span>| <span data-ttu-id="f02a8-146">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="f02a8-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f02a8-147">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="f02a8-147">riskEventStatus</span></span>|<span data-ttu-id="f02a8-148">string</span><span class="sxs-lookup"><span data-stu-id="f02a8-148">string</span></span>| <span data-ttu-id="f02a8-149">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="f02a8-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f02a8-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f02a8-150">riskLevel</span></span>|<span data-ttu-id="f02a8-151">string</span><span class="sxs-lookup"><span data-stu-id="f02a8-151">string</span></span>| <span data-ttu-id="f02a8-152">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f02a8-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f02a8-153">riskEventType</span><span class="sxs-lookup"><span data-stu-id="f02a8-153">riskEventType</span></span>|<span data-ttu-id="f02a8-154">string</span><span class="sxs-lookup"><span data-stu-id="f02a8-154">string</span></span>| <span data-ttu-id="f02a8-155">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="f02a8-155">The type of risk</span></span>|
|<span data-ttu-id="f02a8-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f02a8-156">userDisplayName</span></span>|<span data-ttu-id="f02a8-157">string</span><span class="sxs-lookup"><span data-stu-id="f02a8-157">string</span></span>| <span data-ttu-id="f02a8-158">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="f02a8-158">The name of the user at risk</span></span>|
|<span data-ttu-id="f02a8-159">userId</span><span class="sxs-lookup"><span data-stu-id="f02a8-159">userId</span></span>|<span data-ttu-id="f02a8-160">string</span><span class="sxs-lookup"><span data-stu-id="f02a8-160">string</span></span>| <span data-ttu-id="f02a8-161">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="f02a8-161">The id of the user at risk</span></span>|
|<span data-ttu-id="f02a8-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f02a8-162">userPrincipalName</span></span>|<span data-ttu-id="f02a8-163">string</span><span class="sxs-lookup"><span data-stu-id="f02a8-163">string</span></span>| <span data-ttu-id="f02a8-164">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="f02a8-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f02a8-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f02a8-165">Relationships</span></span>
| <span data-ttu-id="f02a8-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f02a8-166">Relationship</span></span> | <span data-ttu-id="f02a8-167">型</span><span class="sxs-lookup"><span data-stu-id="f02a8-167">Type</span></span>   |<span data-ttu-id="f02a8-168">説明</span><span class="sxs-lookup"><span data-stu-id="f02a8-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f02a8-169">impactedUser</span><span class="sxs-lookup"><span data-stu-id="f02a8-169">impactedUser</span></span>|[<span data-ttu-id="f02a8-170">user</span><span class="sxs-lookup"><span data-stu-id="f02a8-170">user</span></span>](user.md)| <span data-ttu-id="f02a8-p104">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f02a8-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f02a8-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f02a8-173">JSON representation</span></span>

<span data-ttu-id="f02a8-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f02a8-174">Here is a JSON representation of the resource.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
