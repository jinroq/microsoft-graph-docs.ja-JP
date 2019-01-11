---
title: impossibleTravelRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護、ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、に関する該当の記号の完全な情報の間の期間内の場所の間を移動することはできませんが検出されたリスク イベントリスク イベントは、Azure AD のアイデンティティ保護のマニュアルを参照しています。
localization_priority: Normal
ms.openlocfilehash: e9ce064a5ea724b498f3290f630a4169b1aef897
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846453"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="521fc-103">impossibleTravelRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="521fc-103">impossibleTravelRiskEvent resource type</span></span>

> <span data-ttu-id="521fc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="521fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="521fc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="521fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="521fc-106">[Azure Active Directory アイデンティティの保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、記号再起動の完了の間の期間内の場所の間を移動することはできませんが検出されたリスク イベント[Azure AD のアイデンティティ保護マニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)のリスクについての情報が見つかります。</span><span class="sxs-lookup"><span data-stu-id="521fc-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="521fc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="521fc-107">Methods</span></span>

| <span data-ttu-id="521fc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="521fc-108">Method</span></span>           | <span data-ttu-id="521fc-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="521fc-109">Return Type</span></span>    |<span data-ttu-id="521fc-110">説明</span><span class="sxs-lookup"><span data-stu-id="521fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="521fc-111">ImpossibleTravelRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="521fc-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="521fc-112">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="521fc-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="521fc-113">ImpossibleTravelRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="521fc-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="521fc-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="521fc-114">Properties</span></span>
| <span data-ttu-id="521fc-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="521fc-115">Property</span></span>     | <span data-ttu-id="521fc-116">種類</span><span class="sxs-lookup"><span data-stu-id="521fc-116">Type</span></span>   |<span data-ttu-id="521fc-117">説明</span><span class="sxs-lookup"><span data-stu-id="521fc-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="521fc-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="521fc-118">closedDateTime</span></span>|<span data-ttu-id="521fc-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="521fc-119">dateTimeOffset</span></span>| <span data-ttu-id="521fc-120">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="521fc-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="521fc-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="521fc-121">createdDateTime</span></span>|<span data-ttu-id="521fc-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="521fc-122">dateTimeOffset</span></span>| <span data-ttu-id="521fc-123">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="521fc-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="521fc-124">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="521fc-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="521fc-125">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="521fc-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="521fc-126">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="521fc-126">deviceInformation</span></span>|<span data-ttu-id="521fc-127">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-127">string</span></span>| <span data-ttu-id="521fc-128">デバイスに関する情報</span><span class="sxs-lookup"><span data-stu-id="521fc-128">Information about the device</span></span>|
|<span data-ttu-id="521fc-129">ID</span><span class="sxs-lookup"><span data-stu-id="521fc-129">id</span></span>|<span data-ttu-id="521fc-130">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-130">string</span></span>| <span data-ttu-id="521fc-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="521fc-131">Read-only</span></span>|
|<span data-ttu-id="521fc-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="521fc-132">ipAddress</span></span>|<span data-ttu-id="521fc-133">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-133">string</span></span>| <span data-ttu-id="521fc-134">2 つ目のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="521fc-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="521fc-135">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="521fc-135">isAtypicalLocation</span></span>|<span data-ttu-id="521fc-136">ブール</span><span class="sxs-lookup"><span data-stu-id="521fc-136">boolean</span></span>| <span data-ttu-id="521fc-137">ユーザーの典型的な場所のいずれかの場合</span><span class="sxs-lookup"><span data-stu-id="521fc-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="521fc-138">location</span><span class="sxs-lookup"><span data-stu-id="521fc-138">location</span></span>|<span data-ttu-id="521fc-139">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-139">string</span></span>| <span data-ttu-id="521fc-140">2 つ目のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="521fc-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="521fc-141">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="521fc-141">previousIPAddress</span></span>|<span data-ttu-id="521fc-142">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-142">string</span></span>| <span data-ttu-id="521fc-143">最初のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="521fc-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="521fc-144">previousLocation</span><span class="sxs-lookup"><span data-stu-id="521fc-144">previousLocation</span></span>|<span data-ttu-id="521fc-145">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-145">string</span></span>| <span data-ttu-id="521fc-146">最初のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="521fc-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="521fc-147">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="521fc-147">previousSigninDateTime</span></span>|<span data-ttu-id="521fc-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="521fc-148">dateTimeOffset</span></span>| <span data-ttu-id="521fc-149">日付と時刻の最初のサインイン</span><span class="sxs-lookup"><span data-stu-id="521fc-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="521fc-150">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="521fc-150">riskEventDateTime</span></span>|<span data-ttu-id="521fc-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="521fc-151">dateTimeOffset</span></span>| <span data-ttu-id="521fc-152">日付と時刻の 2 つ目のサインイン</span><span class="sxs-lookup"><span data-stu-id="521fc-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="521fc-153">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="521fc-153">riskEventStatus</span></span>|<span data-ttu-id="521fc-154">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-154">string</span></span>| <span data-ttu-id="521fc-155">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="521fc-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="521fc-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="521fc-156">riskLevel</span></span>|<span data-ttu-id="521fc-157">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-157">string</span></span>| <span data-ttu-id="521fc-158">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="521fc-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="521fc-159">riskEventType</span><span class="sxs-lookup"><span data-stu-id="521fc-159">riskEventType</span></span>|<span data-ttu-id="521fc-160">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-160">string</span></span>| <span data-ttu-id="521fc-161">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="521fc-161">The type of risk</span></span>|
|<span data-ttu-id="521fc-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="521fc-162">userAgent</span></span>|<span data-ttu-id="521fc-163">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-163">string</span></span>| <span data-ttu-id="521fc-164">ブラウザーのユーザー エージェント文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-164">The browser's user agent string</span></span>|
|<span data-ttu-id="521fc-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="521fc-165">userDisplayName</span></span>|<span data-ttu-id="521fc-166">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-166">string</span></span>| <span data-ttu-id="521fc-167">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="521fc-167">The name of the user at risk</span></span>|
|<span data-ttu-id="521fc-168">userId</span><span class="sxs-lookup"><span data-stu-id="521fc-168">userId</span></span>|<span data-ttu-id="521fc-169">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-169">string</span></span>| <span data-ttu-id="521fc-170">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="521fc-170">The id of the user at risk</span></span>|
|<span data-ttu-id="521fc-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="521fc-171">userPrincipalName</span></span>|<span data-ttu-id="521fc-172">文字列</span><span class="sxs-lookup"><span data-stu-id="521fc-172">string</span></span>| <span data-ttu-id="521fc-173">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="521fc-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="521fc-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="521fc-174">Relationships</span></span>
| <span data-ttu-id="521fc-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="521fc-175">Relationship</span></span> | <span data-ttu-id="521fc-176">型</span><span class="sxs-lookup"><span data-stu-id="521fc-176">Type</span></span>   |<span data-ttu-id="521fc-177">説明</span><span class="sxs-lookup"><span data-stu-id="521fc-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="521fc-178">impactedUser</span><span class="sxs-lookup"><span data-stu-id="521fc-178">impactedUser</span></span>|[<span data-ttu-id="521fc-179">user</span><span class="sxs-lookup"><span data-stu-id="521fc-179">user</span></span>](user.md)| <span data-ttu-id="521fc-p103">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="521fc-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="521fc-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="521fc-182">JSON representation</span></span>

<span data-ttu-id="521fc-183">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="521fc-183">Here is a JSON representation of the resource.</span></span>

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
