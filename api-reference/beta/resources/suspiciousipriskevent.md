---
title: suspiciousIpRiskEvent リソースの種類
description: Azure Active Directory Id 保護場所、アカウントでサインインしようとすると、不審な IP アドレスからによって検出されたリスク イベントです。 リスク イベントの詳細については、Azure AD のアイデンティティ保護のマニュアルを参照しています。
localization_priority: Normal
ms.openlocfilehash: fff23d3034267adc56f3611f22a181ac415499cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822121"
---
# <a name="suspiciousipriskevent-resource-type"></a><span data-ttu-id="f0a0e-104">suspiciousIpRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0a0e-104">suspiciousIpRiskEvent resource type</span></span>

> <span data-ttu-id="f0a0e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0a0e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0a0e-107">場所、アカウントでサインインしようとすると、不審な IP アドレスから[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="f0a0e-108">リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="f0a0e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f0a0e-109">Methods</span></span>

| <span data-ttu-id="f0a0e-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f0a0e-110">Method</span></span>           | <span data-ttu-id="f0a0e-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f0a0e-111">Return Type</span></span>    |<span data-ttu-id="f0a0e-112">説明</span><span class="sxs-lookup"><span data-stu-id="f0a0e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0a0e-113">SuspiciousIpRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-113">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="f0a0e-114">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0a0e-114">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="f0a0e-115">SuspiciousIpRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-115">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0a0e-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0a0e-116">Properties</span></span>
| <span data-ttu-id="f0a0e-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0a0e-117">Property</span></span>     | <span data-ttu-id="f0a0e-118">種類</span><span class="sxs-lookup"><span data-stu-id="f0a0e-118">Type</span></span>   |<span data-ttu-id="f0a0e-119">説明</span><span class="sxs-lookup"><span data-stu-id="f0a0e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0a0e-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0a0e-120">closedDateTime</span></span>|<span data-ttu-id="f0a0e-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0a0e-121">dateTimeOffset</span></span>| <span data-ttu-id="f0a0e-122">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="f0a0e-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f0a0e-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0a0e-123">createdDateTime</span></span>|<span data-ttu-id="f0a0e-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0a0e-124">dateTimeOffset</span></span>| <span data-ttu-id="f0a0e-125">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="f0a0e-126">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f0a0e-127">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f0a0e-128">ID</span><span class="sxs-lookup"><span data-stu-id="f0a0e-128">id</span></span>|<span data-ttu-id="f0a0e-129">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-129">string</span></span>| <span data-ttu-id="f0a0e-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-130">Read-only</span></span>|
|<span data-ttu-id="f0a0e-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f0a0e-131">ipAddress</span></span>|<span data-ttu-id="f0a0e-132">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-132">string</span></span>| <span data-ttu-id="f0a0e-133">サインイン用の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="f0a0e-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="f0a0e-134">location</span><span class="sxs-lookup"><span data-stu-id="f0a0e-134">location</span></span>|<span data-ttu-id="f0a0e-135">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-135">string</span></span>| <span data-ttu-id="f0a0e-136">サインイン用の IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="f0a0e-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="f0a0e-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="f0a0e-137">riskEventDateTime</span></span>|<span data-ttu-id="f0a0e-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0a0e-138">dateTimeOffset</span></span>| <span data-ttu-id="f0a0e-139">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="f0a0e-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f0a0e-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="f0a0e-140">riskEventStatus</span></span>|<span data-ttu-id="f0a0e-141">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-141">string</span></span>| <span data-ttu-id="f0a0e-142">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f0a0e-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f0a0e-143">riskLevel</span></span>|<span data-ttu-id="f0a0e-144">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-144">string</span></span>| <span data-ttu-id="f0a0e-145">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f0a0e-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="f0a0e-146">riskEventType</span></span>|<span data-ttu-id="f0a0e-147">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-147">string</span></span>| <span data-ttu-id="f0a0e-148">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="f0a0e-148">The type of risk</span></span>|
|<span data-ttu-id="f0a0e-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0a0e-149">userDisplayName</span></span>|<span data-ttu-id="f0a0e-150">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-150">string</span></span>| <span data-ttu-id="f0a0e-151">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="f0a0e-151">The name of the user at risk</span></span>|
|<span data-ttu-id="f0a0e-152">userId</span><span class="sxs-lookup"><span data-stu-id="f0a0e-152">userId</span></span>|<span data-ttu-id="f0a0e-153">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-153">string</span></span>| <span data-ttu-id="f0a0e-154">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="f0a0e-154">The id of the user at risk</span></span>|
|<span data-ttu-id="f0a0e-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0a0e-155">userPrincipalName</span></span>|<span data-ttu-id="f0a0e-156">文字列</span><span class="sxs-lookup"><span data-stu-id="f0a0e-156">string</span></span>| <span data-ttu-id="f0a0e-157">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="f0a0e-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0a0e-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0a0e-158">Relationships</span></span>
| <span data-ttu-id="f0a0e-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0a0e-159">Relationship</span></span> | <span data-ttu-id="f0a0e-160">型</span><span class="sxs-lookup"><span data-stu-id="f0a0e-160">Type</span></span>   |<span data-ttu-id="f0a0e-161">説明</span><span class="sxs-lookup"><span data-stu-id="f0a0e-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0a0e-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="f0a0e-162">impactedUser</span></span>|[<span data-ttu-id="f0a0e-163">user</span><span class="sxs-lookup"><span data-stu-id="f0a0e-163">user</span></span>](user.md)| <span data-ttu-id="f0a0e-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0a0e-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0a0e-166">JSON representation</span></span>

<span data-ttu-id="f0a0e-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0a0e-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
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
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
