---
title: locatedRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護場所データに基づくによって検出されたリスク イベントです。 あるリスク イベントの種類は次のとおりです。
ms.openlocfilehash: e84cff5985905977b6b1eeb75a9ef9703a2a2078
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069398"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="1e813-104">locatedRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e813-104">locatedRiskEvent resource type</span></span>

> <span data-ttu-id="1e813-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e813-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e813-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e813-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e813-107">場所データに基づく[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="1e813-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="1e813-108">あるリスク イベントの種類は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1e813-108">Located risk event types include:</span></span>
* [<span data-ttu-id="1e813-109">匿名の IP アドレスからサインイン</span><span class="sxs-lookup"><span data-stu-id="1e813-109">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="1e813-110">マルウェアに感染したデバイスからのサインインの問題</span><span class="sxs-lookup"><span data-stu-id="1e813-110">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="1e813-111">典型的な場所に旅行を不可能になります。</span><span class="sxs-lookup"><span data-stu-id="1e813-111">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="1e813-112">不審な IP アドレスからサインイン</span><span class="sxs-lookup"><span data-stu-id="1e813-112">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="1e813-113">[未知の場所からサインイン](unfamiliarlocationriskevent.md)リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="1e813-113">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="1e813-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e813-114">Methods</span></span>

| <span data-ttu-id="1e813-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e813-115">Method</span></span>           | <span data-ttu-id="1e813-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1e813-116">Return Type</span></span>    |<span data-ttu-id="1e813-117">説明</span><span class="sxs-lookup"><span data-stu-id="1e813-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e813-118">LocatedRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="1e813-118">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="1e813-119">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1e813-119">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="1e813-120">LocatedRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e813-120">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1e813-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e813-121">Properties</span></span>
| <span data-ttu-id="1e813-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e813-122">Property</span></span>     | <span data-ttu-id="1e813-123">型</span><span class="sxs-lookup"><span data-stu-id="1e813-123">Type</span></span>   |<span data-ttu-id="1e813-124">説明</span><span class="sxs-lookup"><span data-stu-id="1e813-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e813-125">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e813-125">closedDateTime</span></span>|<span data-ttu-id="1e813-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e813-126">dateTimeOffset</span></span>| <span data-ttu-id="1e813-127">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="1e813-127">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="1e813-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e813-128">createdDateTime</span></span>|<span data-ttu-id="1e813-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e813-129">dateTimeOffset</span></span>| <span data-ttu-id="1e813-130">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="1e813-130">The date and time that the risk event was created.</span></span> <span data-ttu-id="1e813-131">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="1e813-131">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="1e813-132">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="1e813-132">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="1e813-133">ID</span><span class="sxs-lookup"><span data-stu-id="1e813-133">id</span></span>|<span data-ttu-id="1e813-134">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-134">string</span></span>| <span data-ttu-id="1e813-135">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="1e813-135">Read-only</span></span>|
|<span data-ttu-id="1e813-136">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1e813-136">ipAddress</span></span>|<span data-ttu-id="1e813-137">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-137">string</span></span>| <span data-ttu-id="1e813-138">サインイン用の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="1e813-138">The IP address of the sign-in</span></span>|
|<span data-ttu-id="1e813-139">location</span><span class="sxs-lookup"><span data-stu-id="1e813-139">location</span></span>|<span data-ttu-id="1e813-140">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-140">string</span></span>| <span data-ttu-id="1e813-141">サインイン用の IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="1e813-141">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="1e813-142">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="1e813-142">riskEventDateTime</span></span>|<span data-ttu-id="1e813-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e813-143">dateTimeOffset</span></span>| <span data-ttu-id="1e813-144">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="1e813-144">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="1e813-145">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="1e813-145">riskEventStatus</span></span>|<span data-ttu-id="1e813-146">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-146">string</span></span>| <span data-ttu-id="1e813-147">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="1e813-147">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="1e813-148">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1e813-148">riskLevel</span></span>|<span data-ttu-id="1e813-149">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-149">string</span></span>| <span data-ttu-id="1e813-150">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="1e813-150">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="1e813-151">riskEventType</span><span class="sxs-lookup"><span data-stu-id="1e813-151">riskEventType</span></span>|<span data-ttu-id="1e813-152">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-152">string</span></span>| <span data-ttu-id="1e813-153">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="1e813-153">The type of risk</span></span>|
|<span data-ttu-id="1e813-154">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1e813-154">userDisplayName</span></span>|<span data-ttu-id="1e813-155">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-155">string</span></span>| <span data-ttu-id="1e813-156">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="1e813-156">The name of the user at risk</span></span>|
|<span data-ttu-id="1e813-157">userId</span><span class="sxs-lookup"><span data-stu-id="1e813-157">userId</span></span>|<span data-ttu-id="1e813-158">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-158">string</span></span>| <span data-ttu-id="1e813-159">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="1e813-159">The id of the user at risk</span></span>|
|<span data-ttu-id="1e813-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1e813-160">userPrincipalName</span></span>|<span data-ttu-id="1e813-161">文字列</span><span class="sxs-lookup"><span data-stu-id="1e813-161">string</span></span>| <span data-ttu-id="1e813-162">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="1e813-162">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e813-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e813-163">Relationships</span></span>
| <span data-ttu-id="1e813-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e813-164">Relationship</span></span> | <span data-ttu-id="1e813-165">型</span><span class="sxs-lookup"><span data-stu-id="1e813-165">Type</span></span>   |<span data-ttu-id="1e813-166">説明</span><span class="sxs-lookup"><span data-stu-id="1e813-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e813-167">impactedUser</span><span class="sxs-lookup"><span data-stu-id="1e813-167">impactedUser</span></span>|[<span data-ttu-id="1e813-168">user</span><span class="sxs-lookup"><span data-stu-id="1e813-168">user</span></span>](user.md)| <span data-ttu-id="1e813-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1e813-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e813-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e813-171">JSON representation</span></span>

<span data-ttu-id="1e813-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e813-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locatedRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->