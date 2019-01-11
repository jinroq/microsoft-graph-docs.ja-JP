---
title: unfamiliarLocationRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護場所、アカウントでサインインしようとするとそのユーザーの新しい場所からによって検出されたリスク イベントです。 リスク イベントの詳細については、Azure AD のアイデンティティ保護のマニュアルを参照しています。
localization_priority: Normal
ms.openlocfilehash: 130d68bfb23bdb23b6a9de81fa988d38db1d8c10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868741"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="1f2a1-104">unfamiliarLocationRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f2a1-104">unfamiliarLocationRiskEvent resource type</span></span>

> <span data-ttu-id="1f2a1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f2a1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f2a1-107">[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)場所、アカウントでサインインしようとするとそのユーザーの新しい場所からによって検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="1f2a1-108">リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="1f2a1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f2a1-109">Methods</span></span>

| <span data-ttu-id="1f2a1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f2a1-110">Method</span></span>           | <span data-ttu-id="1f2a1-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1f2a1-111">Return Type</span></span>    |<span data-ttu-id="1f2a1-112">説明</span><span class="sxs-lookup"><span data-stu-id="1f2a1-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f2a1-113">UnfamiliarLocationRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-113">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="1f2a1-114">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1f2a1-114">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="1f2a1-115">UnfamiliarLocationRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-115">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f2a1-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f2a1-116">Properties</span></span>
| <span data-ttu-id="1f2a1-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f2a1-117">Property</span></span>     | <span data-ttu-id="1f2a1-118">種類</span><span class="sxs-lookup"><span data-stu-id="1f2a1-118">Type</span></span>   |<span data-ttu-id="1f2a1-119">説明</span><span class="sxs-lookup"><span data-stu-id="1f2a1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f2a1-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f2a1-120">closedDateTime</span></span>|<span data-ttu-id="1f2a1-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f2a1-121">dateTimeOffset</span></span>| <span data-ttu-id="1f2a1-122">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="1f2a1-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="1f2a1-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f2a1-123">createdDateTime</span></span>|<span data-ttu-id="1f2a1-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f2a1-124">dateTimeOffset</span></span>| <span data-ttu-id="1f2a1-125">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="1f2a1-126">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="1f2a1-127">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="1f2a1-128">ID</span><span class="sxs-lookup"><span data-stu-id="1f2a1-128">id</span></span>|<span data-ttu-id="1f2a1-129">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-129">string</span></span>| <span data-ttu-id="1f2a1-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-130">Read-only</span></span>|
|<span data-ttu-id="1f2a1-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1f2a1-131">ipAddress</span></span>|<span data-ttu-id="1f2a1-132">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-132">string</span></span>| <span data-ttu-id="1f2a1-133">サインイン用の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="1f2a1-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="1f2a1-134">location</span><span class="sxs-lookup"><span data-stu-id="1f2a1-134">location</span></span>|<span data-ttu-id="1f2a1-135">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-135">string</span></span>| <span data-ttu-id="1f2a1-136">サインイン用の IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="1f2a1-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="1f2a1-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="1f2a1-137">riskEventDateTime</span></span>|<span data-ttu-id="1f2a1-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f2a1-138">dateTimeOffset</span></span>| <span data-ttu-id="1f2a1-139">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="1f2a1-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="1f2a1-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="1f2a1-140">riskEventStatus</span></span>|<span data-ttu-id="1f2a1-141">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-141">string</span></span>| <span data-ttu-id="1f2a1-142">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="1f2a1-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1f2a1-143">riskLevel</span></span>|<span data-ttu-id="1f2a1-144">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-144">string</span></span>| <span data-ttu-id="1f2a1-145">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="1f2a1-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="1f2a1-146">riskEventType</span></span>|<span data-ttu-id="1f2a1-147">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-147">string</span></span>| <span data-ttu-id="1f2a1-148">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="1f2a1-148">The type of risk</span></span>|
|<span data-ttu-id="1f2a1-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1f2a1-149">userDisplayName</span></span>|<span data-ttu-id="1f2a1-150">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-150">string</span></span>| <span data-ttu-id="1f2a1-151">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="1f2a1-151">The name of the user at risk</span></span>|
|<span data-ttu-id="1f2a1-152">userId</span><span class="sxs-lookup"><span data-stu-id="1f2a1-152">userId</span></span>|<span data-ttu-id="1f2a1-153">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-153">string</span></span>| <span data-ttu-id="1f2a1-154">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="1f2a1-154">The id of the user at risk</span></span>|
|<span data-ttu-id="1f2a1-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1f2a1-155">userPrincipalName</span></span>|<span data-ttu-id="1f2a1-156">文字列</span><span class="sxs-lookup"><span data-stu-id="1f2a1-156">string</span></span>| <span data-ttu-id="1f2a1-157">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="1f2a1-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f2a1-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f2a1-158">Relationships</span></span>
| <span data-ttu-id="1f2a1-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f2a1-159">Relationship</span></span> | <span data-ttu-id="1f2a1-160">型</span><span class="sxs-lookup"><span data-stu-id="1f2a1-160">Type</span></span>   |<span data-ttu-id="1f2a1-161">説明</span><span class="sxs-lookup"><span data-stu-id="1f2a1-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f2a1-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="1f2a1-162">impactedUser</span></span>|[<span data-ttu-id="1f2a1-163">user</span><span class="sxs-lookup"><span data-stu-id="1f2a1-163">user</span></span>](user.md)| <span data-ttu-id="1f2a1-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f2a1-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f2a1-166">JSON representation</span></span>

<span data-ttu-id="1f2a1-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f2a1-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
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
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
