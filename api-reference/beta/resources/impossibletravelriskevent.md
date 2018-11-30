---
title: impossibleTravelRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護、ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、に関する該当の記号の完全な情報の間の期間内の場所の間を移動することはできませんが検出されたリスク イベントリスク イベントは、Azure AD のアイデンティティ保護のマニュアルを参照しています。
ms.openlocfilehash: 38e61927121f520e79fd1fec8b8e6443fa8b76e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066785"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="e1150-103">impossibleTravelRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1150-103">impossibleTravelRiskEvent resource type</span></span>

> <span data-ttu-id="e1150-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1150-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1150-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1150-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1150-106">[Azure Active Directory アイデンティティの保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、記号再起動の完了の間の期間内の場所の間を移動することはできませんが検出されたリスク イベント[Azure AD のアイデンティティ保護マニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)のリスクについての情報が見つかります。</span><span class="sxs-lookup"><span data-stu-id="e1150-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="e1150-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1150-107">Methods</span></span>

| <span data-ttu-id="e1150-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1150-108">Method</span></span>           | <span data-ttu-id="e1150-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e1150-109">Return Type</span></span>    |<span data-ttu-id="e1150-110">説明</span><span class="sxs-lookup"><span data-stu-id="e1150-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1150-111">ImpossibleTravelRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="e1150-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="e1150-112">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e1150-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="e1150-113">ImpossibleTravelRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1150-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1150-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1150-114">Properties</span></span>
| <span data-ttu-id="e1150-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1150-115">Property</span></span>     | <span data-ttu-id="e1150-116">型</span><span class="sxs-lookup"><span data-stu-id="e1150-116">Type</span></span>   |<span data-ttu-id="e1150-117">説明</span><span class="sxs-lookup"><span data-stu-id="e1150-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1150-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1150-118">closedDateTime</span></span>|<span data-ttu-id="e1150-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1150-119">dateTimeOffset</span></span>| <span data-ttu-id="e1150-120">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="e1150-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e1150-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1150-121">createdDateTime</span></span>|<span data-ttu-id="e1150-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1150-122">dateTimeOffset</span></span>| <span data-ttu-id="e1150-123">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="e1150-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="e1150-124">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="e1150-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e1150-125">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="e1150-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e1150-126">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="e1150-126">deviceInformation</span></span>|<span data-ttu-id="e1150-127">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-127">string</span></span>| <span data-ttu-id="e1150-128">デバイスに関する情報</span><span class="sxs-lookup"><span data-stu-id="e1150-128">Information about the device</span></span>|
|<span data-ttu-id="e1150-129">ID</span><span class="sxs-lookup"><span data-stu-id="e1150-129">id</span></span>|<span data-ttu-id="e1150-130">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-130">string</span></span>| <span data-ttu-id="e1150-131">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="e1150-131">Read-only</span></span>|
|<span data-ttu-id="e1150-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e1150-132">ipAddress</span></span>|<span data-ttu-id="e1150-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-133">string</span></span>| <span data-ttu-id="e1150-134">2 つ目のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="e1150-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="e1150-135">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="e1150-135">isAtypicalLocation</span></span>|<span data-ttu-id="e1150-136">ブール</span><span class="sxs-lookup"><span data-stu-id="e1150-136">boolean</span></span>| <span data-ttu-id="e1150-137">ユーザーの典型的な場所のいずれかの場合</span><span class="sxs-lookup"><span data-stu-id="e1150-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="e1150-138">location</span><span class="sxs-lookup"><span data-stu-id="e1150-138">location</span></span>|<span data-ttu-id="e1150-139">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-139">string</span></span>| <span data-ttu-id="e1150-140">2 つ目のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="e1150-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="e1150-141">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="e1150-141">previousIPAddress</span></span>|<span data-ttu-id="e1150-142">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-142">string</span></span>| <span data-ttu-id="e1150-143">最初のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="e1150-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="e1150-144">previousLocation</span><span class="sxs-lookup"><span data-stu-id="e1150-144">previousLocation</span></span>|<span data-ttu-id="e1150-145">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-145">string</span></span>| <span data-ttu-id="e1150-146">最初のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="e1150-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="e1150-147">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="e1150-147">previousSigninDateTime</span></span>|<span data-ttu-id="e1150-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1150-148">dateTimeOffset</span></span>| <span data-ttu-id="e1150-149">日付と時刻の最初のサインイン</span><span class="sxs-lookup"><span data-stu-id="e1150-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="e1150-150">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="e1150-150">riskEventDateTime</span></span>|<span data-ttu-id="e1150-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1150-151">dateTimeOffset</span></span>| <span data-ttu-id="e1150-152">日付と時刻の 2 つ目のサインイン</span><span class="sxs-lookup"><span data-stu-id="e1150-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="e1150-153">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="e1150-153">riskEventStatus</span></span>|<span data-ttu-id="e1150-154">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-154">string</span></span>| <span data-ttu-id="e1150-155">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="e1150-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e1150-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e1150-156">riskLevel</span></span>|<span data-ttu-id="e1150-157">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-157">string</span></span>| <span data-ttu-id="e1150-158">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e1150-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e1150-159">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e1150-159">riskEventType</span></span>|<span data-ttu-id="e1150-160">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-160">string</span></span>| <span data-ttu-id="e1150-161">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="e1150-161">The type of risk</span></span>|
|<span data-ttu-id="e1150-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="e1150-162">userAgent</span></span>|<span data-ttu-id="e1150-163">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-163">string</span></span>| <span data-ttu-id="e1150-164">ブラウザーのユーザー エージェント文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-164">The browser's user agent string</span></span>|
|<span data-ttu-id="e1150-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e1150-165">userDisplayName</span></span>|<span data-ttu-id="e1150-166">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-166">string</span></span>| <span data-ttu-id="e1150-167">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="e1150-167">The name of the user at risk</span></span>|
|<span data-ttu-id="e1150-168">userId</span><span class="sxs-lookup"><span data-stu-id="e1150-168">userId</span></span>|<span data-ttu-id="e1150-169">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-169">string</span></span>| <span data-ttu-id="e1150-170">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="e1150-170">The id of the user at risk</span></span>|
|<span data-ttu-id="e1150-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1150-171">userPrincipalName</span></span>|<span data-ttu-id="e1150-172">文字列</span><span class="sxs-lookup"><span data-stu-id="e1150-172">string</span></span>| <span data-ttu-id="e1150-173">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="e1150-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1150-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1150-174">Relationships</span></span>
| <span data-ttu-id="e1150-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1150-175">Relationship</span></span> | <span data-ttu-id="e1150-176">型</span><span class="sxs-lookup"><span data-stu-id="e1150-176">Type</span></span>   |<span data-ttu-id="e1150-177">説明</span><span class="sxs-lookup"><span data-stu-id="e1150-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1150-178">impactedUser</span><span class="sxs-lookup"><span data-stu-id="e1150-178">impactedUser</span></span>|[<span data-ttu-id="e1150-179">user</span><span class="sxs-lookup"><span data-stu-id="e1150-179">user</span></span>](user.md)| <span data-ttu-id="e1150-p103">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e1150-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1150-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1150-182">JSON representation</span></span>

<span data-ttu-id="e1150-183">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e1150-183">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->