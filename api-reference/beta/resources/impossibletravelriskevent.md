---
title: impossibleTravelRiskEvent リソースの種類
description: ユーザーにとって特殊な場所から2つのアカウントのサインインが発生する、Azure Active Directory id 保護によって検出されたリスクイベント。また、サインイン間の期間内にある場所間を移動できません。詳細な情報リスクイベントについては、「Azure AD Identity Protection」のドキュメントを参照してください。
localization_priority: Normal
ms.openlocfilehash: d086a6fc127649da10184ae0396a2c58ee82964e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333604"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="07496-103">impossibleTravelRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="07496-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07496-104">ユーザーにとって特殊な場所から2つのアカウントのサインインが発生する[Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されるリスクイベント。これは、サインイン間の期間内で場所間を移動できません。リスクイベントに関する情報については、「 [Azure AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="07496-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="07496-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="07496-105">Methods</span></span>

| <span data-ttu-id="07496-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="07496-106">Method</span></span>           | <span data-ttu-id="07496-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="07496-107">Return Type</span></span>    |<span data-ttu-id="07496-108">説明</span><span class="sxs-lookup"><span data-stu-id="07496-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07496-109">impossibleTravelRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="07496-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="07496-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="07496-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="07496-111">impossibleTravelRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="07496-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07496-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07496-112">Properties</span></span>
| <span data-ttu-id="07496-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07496-113">Property</span></span>     | <span data-ttu-id="07496-114">型</span><span class="sxs-lookup"><span data-stu-id="07496-114">Type</span></span>   |<span data-ttu-id="07496-115">説明</span><span class="sxs-lookup"><span data-stu-id="07496-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07496-116">closeddatetime</span><span class="sxs-lookup"><span data-stu-id="07496-116">closedDateTime</span></span>|<span data-ttu-id="07496-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07496-117">dateTimeOffset</span></span>| <span data-ttu-id="07496-118">リスクイベントが終了した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="07496-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="07496-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07496-119">createdDateTime</span></span>|<span data-ttu-id="07496-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07496-120">dateTimeOffset</span></span>| <span data-ttu-id="07496-121">リスクイベントが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="07496-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="07496-122">これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。</span><span class="sxs-lookup"><span data-stu-id="07496-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="07496-123">これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="07496-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="07496-124">deviceinformation</span><span class="sxs-lookup"><span data-stu-id="07496-124">deviceInformation</span></span>|<span data-ttu-id="07496-125">string</span><span class="sxs-lookup"><span data-stu-id="07496-125">string</span></span>| <span data-ttu-id="07496-126">デバイスに関する情報</span><span class="sxs-lookup"><span data-stu-id="07496-126">Information about the device</span></span>|
|<span data-ttu-id="07496-127">id</span><span class="sxs-lookup"><span data-stu-id="07496-127">id</span></span>|<span data-ttu-id="07496-128">文字列</span><span class="sxs-lookup"><span data-stu-id="07496-128">string</span></span>| <span data-ttu-id="07496-129">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="07496-129">Read-only</span></span>|
|<span data-ttu-id="07496-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="07496-130">ipAddress</span></span>|<span data-ttu-id="07496-131">string</span><span class="sxs-lookup"><span data-stu-id="07496-131">string</span></span>| <span data-ttu-id="07496-132">2番目のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="07496-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="07496-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="07496-133">isAtypicalLocation</span></span>|<span data-ttu-id="07496-134">boolean</span><span class="sxs-lookup"><span data-stu-id="07496-134">boolean</span></span>| <span data-ttu-id="07496-135">ユーザーのいずれかの場所が例外的である場合</span><span class="sxs-lookup"><span data-stu-id="07496-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="07496-136">location</span><span class="sxs-lookup"><span data-stu-id="07496-136">location</span></span>|<span data-ttu-id="07496-137">string</span><span class="sxs-lookup"><span data-stu-id="07496-137">string</span></span>| <span data-ttu-id="07496-138">2番目のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="07496-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="07496-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="07496-139">previousIPAddress</span></span>|<span data-ttu-id="07496-140">string</span><span class="sxs-lookup"><span data-stu-id="07496-140">string</span></span>| <span data-ttu-id="07496-141">最初のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="07496-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="07496-142">previousLocation</span><span class="sxs-lookup"><span data-stu-id="07496-142">previousLocation</span></span>|<span data-ttu-id="07496-143">string</span><span class="sxs-lookup"><span data-stu-id="07496-143">string</span></span>| <span data-ttu-id="07496-144">最初のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="07496-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="07496-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="07496-145">previousSigninDateTime</span></span>|<span data-ttu-id="07496-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07496-146">dateTimeOffset</span></span>| <span data-ttu-id="07496-147">最初のサインインの日付と時刻</span><span class="sxs-lookup"><span data-stu-id="07496-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="07496-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="07496-148">riskEventDateTime</span></span>|<span data-ttu-id="07496-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07496-149">dateTimeOffset</span></span>| <span data-ttu-id="07496-150">2番目のサインインの日付と時刻</span><span class="sxs-lookup"><span data-stu-id="07496-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="07496-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="07496-151">riskEventStatus</span></span>|<span data-ttu-id="07496-152">string</span><span class="sxs-lookup"><span data-stu-id="07496-152">string</span></span>| <span data-ttu-id="07496-153">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="07496-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="07496-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="07496-154">riskLevel</span></span>|<span data-ttu-id="07496-155">string</span><span class="sxs-lookup"><span data-stu-id="07496-155">string</span></span>| <span data-ttu-id="07496-156">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="07496-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="07496-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="07496-157">riskEventType</span></span>|<span data-ttu-id="07496-158">string</span><span class="sxs-lookup"><span data-stu-id="07496-158">string</span></span>| <span data-ttu-id="07496-159">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="07496-159">The type of risk</span></span>|
|<span data-ttu-id="07496-160">userAgent</span><span class="sxs-lookup"><span data-stu-id="07496-160">userAgent</span></span>|<span data-ttu-id="07496-161">string</span><span class="sxs-lookup"><span data-stu-id="07496-161">string</span></span>| <span data-ttu-id="07496-162">ブラウザーのユーザーエージェント文字列</span><span class="sxs-lookup"><span data-stu-id="07496-162">The browser's user agent string</span></span>|
|<span data-ttu-id="07496-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="07496-163">userDisplayName</span></span>|<span data-ttu-id="07496-164">string</span><span class="sxs-lookup"><span data-stu-id="07496-164">string</span></span>| <span data-ttu-id="07496-165">リスクのあるユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="07496-165">The name of the user at risk</span></span>|
|<span data-ttu-id="07496-166">userId</span><span class="sxs-lookup"><span data-stu-id="07496-166">userId</span></span>|<span data-ttu-id="07496-167">string</span><span class="sxs-lookup"><span data-stu-id="07496-167">string</span></span>| <span data-ttu-id="07496-168">リスクがあるユーザーの id</span><span class="sxs-lookup"><span data-stu-id="07496-168">The id of the user at risk</span></span>|
|<span data-ttu-id="07496-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="07496-169">userPrincipalName</span></span>|<span data-ttu-id="07496-170">string</span><span class="sxs-lookup"><span data-stu-id="07496-170">string</span></span>| <span data-ttu-id="07496-171">リスクがあるユーザーのユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="07496-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="07496-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07496-172">Relationships</span></span>
| <span data-ttu-id="07496-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07496-173">Relationship</span></span> | <span data-ttu-id="07496-174">型</span><span class="sxs-lookup"><span data-stu-id="07496-174">Type</span></span>   |<span data-ttu-id="07496-175">説明</span><span class="sxs-lookup"><span data-stu-id="07496-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07496-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="07496-176">impactedUser</span></span>|[<span data-ttu-id="07496-177">user</span><span class="sxs-lookup"><span data-stu-id="07496-177">user</span></span>](user.md)| <span data-ttu-id="07496-p102">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="07496-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07496-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07496-180">JSON representation</span></span>

<span data-ttu-id="07496-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="07496-181">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
