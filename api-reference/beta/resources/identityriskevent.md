---
title: identityRiskEvent リソースの種類
description: Azure Active Directory id 保護によって検出されたリスクイベント。 これは、各固有のリスクイベントの種類の基本型です。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506401"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="ddceb-104">identityRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ddceb-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddceb-105">[Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスクイベント。</span><span class="sxs-lookup"><span data-stu-id="ddceb-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="ddceb-106">これは、各固有のリスクイベントの種類の基本型です。</span><span class="sxs-lookup"><span data-stu-id="ddceb-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="ddceb-107">イベントの種類</span><span class="sxs-lookup"><span data-stu-id="ddceb-107">Event type</span></span>         | <span data-ttu-id="ddceb-108">説明</span><span class="sxs-lookup"><span data-stu-id="ddceb-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="ddceb-109">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ddceb-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="ddceb-110">匿名 IP アドレスからのサインイン。</span><span class="sxs-lookup"><span data-stu-id="ddceb-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="ddceb-111">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ddceb-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="ddceb-112">マルウェアに感染したデバイスからのサインイン。</span><span class="sxs-lookup"><span data-stu-id="ddceb-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="ddceb-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ddceb-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="ddceb-114">例外的でない場所への移動は不可能です。</span><span class="sxs-lookup"><span data-stu-id="ddceb-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="ddceb-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ddceb-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="ddceb-116">資格情報がリークしたユーザー。</span><span class="sxs-lookup"><span data-stu-id="ddceb-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="ddceb-117">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ddceb-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="ddceb-118">疑わしい IP アドレスからのサインイン。</span><span class="sxs-lookup"><span data-stu-id="ddceb-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="ddceb-119">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ddceb-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="ddceb-120">見慣れない場所からのサインイン。</span><span class="sxs-lookup"><span data-stu-id="ddceb-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="ddceb-121">リスクイベントに関する詳細な情報については、「 [Azure AD Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)」のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddceb-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="ddceb-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddceb-122">Methods</span></span>

| <span data-ttu-id="ddceb-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddceb-123">Method</span></span>           | <span data-ttu-id="ddceb-124">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ddceb-124">Return Type</span></span>    |<span data-ttu-id="ddceb-125">説明</span><span class="sxs-lookup"><span data-stu-id="ddceb-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ddceb-126">identityRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="ddceb-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="ddceb-127">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ddceb-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="ddceb-128">identityRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ddceb-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddceb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddceb-129">Properties</span></span>
| <span data-ttu-id="ddceb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddceb-130">Property</span></span>     | <span data-ttu-id="ddceb-131">型</span><span class="sxs-lookup"><span data-stu-id="ddceb-131">Type</span></span>   |<span data-ttu-id="ddceb-132">説明</span><span class="sxs-lookup"><span data-stu-id="ddceb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddceb-133">closeddatetime</span><span class="sxs-lookup"><span data-stu-id="ddceb-133">closedDateTime</span></span>|<span data-ttu-id="ddceb-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddceb-134">dateTimeOffset</span></span>| <span data-ttu-id="ddceb-135">リスクイベントが終了した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="ddceb-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="ddceb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddceb-136">createdDateTime</span></span>|<span data-ttu-id="ddceb-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddceb-137">dateTimeOffset</span></span>| <span data-ttu-id="ddceb-138">リスクイベントが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ddceb-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="ddceb-139">これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。</span><span class="sxs-lookup"><span data-stu-id="ddceb-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="ddceb-140">これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="ddceb-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="ddceb-141">id</span><span class="sxs-lookup"><span data-stu-id="ddceb-141">id</span></span>|<span data-ttu-id="ddceb-142">string</span><span class="sxs-lookup"><span data-stu-id="ddceb-142">string</span></span>| <span data-ttu-id="ddceb-143">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="ddceb-143">Read-only</span></span>|
|<span data-ttu-id="ddceb-144">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="ddceb-144">riskEventDateTime</span></span>|<span data-ttu-id="ddceb-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddceb-145">dateTimeOffset</span></span>| <span data-ttu-id="ddceb-146">リスクイベントが発生した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="ddceb-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="ddceb-147">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="ddceb-147">riskEventStatus</span></span>|<span data-ttu-id="ddceb-148">string</span><span class="sxs-lookup"><span data-stu-id="ddceb-148">string</span></span>| <span data-ttu-id="ddceb-149">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="ddceb-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="ddceb-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ddceb-150">riskLevel</span></span>|<span data-ttu-id="ddceb-151">string</span><span class="sxs-lookup"><span data-stu-id="ddceb-151">string</span></span>| <span data-ttu-id="ddceb-152">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="ddceb-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="ddceb-153">riskEventType</span><span class="sxs-lookup"><span data-stu-id="ddceb-153">riskEventType</span></span>|<span data-ttu-id="ddceb-154">string</span><span class="sxs-lookup"><span data-stu-id="ddceb-154">string</span></span>| <span data-ttu-id="ddceb-155">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="ddceb-155">The type of risk</span></span>|
|<span data-ttu-id="ddceb-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ddceb-156">userDisplayName</span></span>|<span data-ttu-id="ddceb-157">string</span><span class="sxs-lookup"><span data-stu-id="ddceb-157">string</span></span>| <span data-ttu-id="ddceb-158">リスクのあるユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="ddceb-158">The name of the user at risk</span></span>|
|<span data-ttu-id="ddceb-159">userId</span><span class="sxs-lookup"><span data-stu-id="ddceb-159">userId</span></span>|<span data-ttu-id="ddceb-160">string</span><span class="sxs-lookup"><span data-stu-id="ddceb-160">string</span></span>| <span data-ttu-id="ddceb-161">リスクがあるユーザーの id</span><span class="sxs-lookup"><span data-stu-id="ddceb-161">The id of the user at risk</span></span>|
|<span data-ttu-id="ddceb-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ddceb-162">userPrincipalName</span></span>|<span data-ttu-id="ddceb-163">string</span><span class="sxs-lookup"><span data-stu-id="ddceb-163">string</span></span>| <span data-ttu-id="ddceb-164">リスクがあるユーザーのユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="ddceb-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddceb-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddceb-165">Relationships</span></span>
| <span data-ttu-id="ddceb-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddceb-166">Relationship</span></span> | <span data-ttu-id="ddceb-167">型</span><span class="sxs-lookup"><span data-stu-id="ddceb-167">Type</span></span>   |<span data-ttu-id="ddceb-168">説明</span><span class="sxs-lookup"><span data-stu-id="ddceb-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddceb-169">impactedUser</span><span class="sxs-lookup"><span data-stu-id="ddceb-169">impactedUser</span></span>|[<span data-ttu-id="ddceb-170">ユーザー</span><span class="sxs-lookup"><span data-stu-id="ddceb-170">user</span></span>](user.md)| <span data-ttu-id="ddceb-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="ddceb-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ddceb-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddceb-173">JSON representation</span></span>

<span data-ttu-id="ddceb-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ddceb-174">Here is a JSON representation of the resource.</span></span> 

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
