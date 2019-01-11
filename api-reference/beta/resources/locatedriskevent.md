---
title: locatedRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護場所データに基づくによって検出されたリスク イベントです。 あるリスク イベントの種類は次のとおりです。
localization_priority: Normal
ms.openlocfilehash: 256c7a980fb9540e7e80337a5b8aad29fe73f26a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867558"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="10b99-104">locatedRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="10b99-104">locatedRiskEvent resource type</span></span>

> <span data-ttu-id="10b99-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="10b99-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10b99-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10b99-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10b99-107">場所データに基づく[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="10b99-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="10b99-108">あるリスク イベントの種類は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="10b99-108">Located risk event types include:</span></span>
* [<span data-ttu-id="10b99-109">匿名の IP アドレスからサインイン</span><span class="sxs-lookup"><span data-stu-id="10b99-109">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="10b99-110">マルウェアに感染したデバイスからのサインインの問題</span><span class="sxs-lookup"><span data-stu-id="10b99-110">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="10b99-111">典型的な場所に旅行を不可能になります。</span><span class="sxs-lookup"><span data-stu-id="10b99-111">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="10b99-112">不審な IP アドレスからサインイン</span><span class="sxs-lookup"><span data-stu-id="10b99-112">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="10b99-113">[未知の場所からサインイン](unfamiliarlocationriskevent.md)リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="10b99-113">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="10b99-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="10b99-114">Methods</span></span>

| <span data-ttu-id="10b99-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="10b99-115">Method</span></span>           | <span data-ttu-id="10b99-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="10b99-116">Return Type</span></span>    |<span data-ttu-id="10b99-117">説明</span><span class="sxs-lookup"><span data-stu-id="10b99-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10b99-118">LocatedRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="10b99-118">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="10b99-119">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="10b99-119">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="10b99-120">LocatedRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10b99-120">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10b99-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10b99-121">Properties</span></span>
| <span data-ttu-id="10b99-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10b99-122">Property</span></span>     | <span data-ttu-id="10b99-123">種類</span><span class="sxs-lookup"><span data-stu-id="10b99-123">Type</span></span>   |<span data-ttu-id="10b99-124">説明</span><span class="sxs-lookup"><span data-stu-id="10b99-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10b99-125">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="10b99-125">closedDateTime</span></span>|<span data-ttu-id="10b99-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b99-126">dateTimeOffset</span></span>| <span data-ttu-id="10b99-127">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="10b99-127">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="10b99-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10b99-128">createdDateTime</span></span>|<span data-ttu-id="10b99-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b99-129">dateTimeOffset</span></span>| <span data-ttu-id="10b99-130">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="10b99-130">The date and time that the risk event was created.</span></span> <span data-ttu-id="10b99-131">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="10b99-131">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="10b99-132">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="10b99-132">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="10b99-133">ID</span><span class="sxs-lookup"><span data-stu-id="10b99-133">id</span></span>|<span data-ttu-id="10b99-134">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-134">string</span></span>| <span data-ttu-id="10b99-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="10b99-135">Read-only</span></span>|
|<span data-ttu-id="10b99-136">ipAddress</span><span class="sxs-lookup"><span data-stu-id="10b99-136">ipAddress</span></span>|<span data-ttu-id="10b99-137">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-137">string</span></span>| <span data-ttu-id="10b99-138">サインイン用の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="10b99-138">The IP address of the sign-in</span></span>|
|<span data-ttu-id="10b99-139">location</span><span class="sxs-lookup"><span data-stu-id="10b99-139">location</span></span>|<span data-ttu-id="10b99-140">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-140">string</span></span>| <span data-ttu-id="10b99-141">サインイン用の IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="10b99-141">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="10b99-142">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="10b99-142">riskEventDateTime</span></span>|<span data-ttu-id="10b99-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b99-143">dateTimeOffset</span></span>| <span data-ttu-id="10b99-144">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="10b99-144">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="10b99-145">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="10b99-145">riskEventStatus</span></span>|<span data-ttu-id="10b99-146">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-146">string</span></span>| <span data-ttu-id="10b99-147">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="10b99-147">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="10b99-148">riskLevel</span><span class="sxs-lookup"><span data-stu-id="10b99-148">riskLevel</span></span>|<span data-ttu-id="10b99-149">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-149">string</span></span>| <span data-ttu-id="10b99-150">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="10b99-150">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="10b99-151">riskEventType</span><span class="sxs-lookup"><span data-stu-id="10b99-151">riskEventType</span></span>|<span data-ttu-id="10b99-152">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-152">string</span></span>| <span data-ttu-id="10b99-153">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="10b99-153">The type of risk</span></span>|
|<span data-ttu-id="10b99-154">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="10b99-154">userDisplayName</span></span>|<span data-ttu-id="10b99-155">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-155">string</span></span>| <span data-ttu-id="10b99-156">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="10b99-156">The name of the user at risk</span></span>|
|<span data-ttu-id="10b99-157">userId</span><span class="sxs-lookup"><span data-stu-id="10b99-157">userId</span></span>|<span data-ttu-id="10b99-158">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-158">string</span></span>| <span data-ttu-id="10b99-159">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="10b99-159">The id of the user at risk</span></span>|
|<span data-ttu-id="10b99-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10b99-160">userPrincipalName</span></span>|<span data-ttu-id="10b99-161">文字列</span><span class="sxs-lookup"><span data-stu-id="10b99-161">string</span></span>| <span data-ttu-id="10b99-162">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="10b99-162">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="10b99-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="10b99-163">Relationships</span></span>
| <span data-ttu-id="10b99-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="10b99-164">Relationship</span></span> | <span data-ttu-id="10b99-165">型</span><span class="sxs-lookup"><span data-stu-id="10b99-165">Type</span></span>   |<span data-ttu-id="10b99-166">説明</span><span class="sxs-lookup"><span data-stu-id="10b99-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10b99-167">impactedUser</span><span class="sxs-lookup"><span data-stu-id="10b99-167">impactedUser</span></span>|[<span data-ttu-id="10b99-168">user</span><span class="sxs-lookup"><span data-stu-id="10b99-168">user</span></span>](user.md)| <span data-ttu-id="10b99-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="10b99-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10b99-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10b99-171">JSON representation</span></span>

<span data-ttu-id="10b99-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="10b99-172">Here is a JSON representation of the resource.</span></span>

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
