---
title: impossibleTravelRiskEvent リソースの種類
description: ユーザーにとって特殊な場所から2つのアカウントのサインインが発生する、Azure Active Directory id 保護によって検出されたリスクイベント。また、サインイン間の期間内にある場所間を移動できません。詳細な情報リスクイベントについては、「Azure AD Identity Protection」のドキュメントを参照してください。
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548328"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="c174e-103">impossibleTravelRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c174e-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c174e-104">ユーザーにとって特殊な場所から2つのアカウントのサインインが発生する[Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されるリスクイベント。これは、サインイン間の期間内で場所間を移動できません。リスクイベントに関する情報については、「 [Azure AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c174e-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="c174e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c174e-105">Methods</span></span>

| <span data-ttu-id="c174e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c174e-106">Method</span></span>           | <span data-ttu-id="c174e-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c174e-107">Return Type</span></span>    |<span data-ttu-id="c174e-108">説明</span><span class="sxs-lookup"><span data-stu-id="c174e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c174e-109">impossibleTravelRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="c174e-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="c174e-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c174e-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="c174e-111">impossibleTravelRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c174e-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c174e-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c174e-112">Properties</span></span>
| <span data-ttu-id="c174e-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c174e-113">Property</span></span>     | <span data-ttu-id="c174e-114">型</span><span class="sxs-lookup"><span data-stu-id="c174e-114">Type</span></span>   |<span data-ttu-id="c174e-115">説明</span><span class="sxs-lookup"><span data-stu-id="c174e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c174e-116">closeddatetime</span><span class="sxs-lookup"><span data-stu-id="c174e-116">closedDateTime</span></span>|<span data-ttu-id="c174e-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c174e-117">dateTimeOffset</span></span>| <span data-ttu-id="c174e-118">リスクイベントが終了した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="c174e-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c174e-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c174e-119">createdDateTime</span></span>|<span data-ttu-id="c174e-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c174e-120">dateTimeOffset</span></span>| <span data-ttu-id="c174e-121">リスクイベントが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c174e-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="c174e-122">これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。</span><span class="sxs-lookup"><span data-stu-id="c174e-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c174e-123">これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="c174e-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c174e-124">deviceinformation</span><span class="sxs-lookup"><span data-stu-id="c174e-124">deviceInformation</span></span>|<span data-ttu-id="c174e-125">string</span><span class="sxs-lookup"><span data-stu-id="c174e-125">string</span></span>| <span data-ttu-id="c174e-126">デバイスに関する情報</span><span class="sxs-lookup"><span data-stu-id="c174e-126">Information about the device</span></span>|
|<span data-ttu-id="c174e-127">id</span><span class="sxs-lookup"><span data-stu-id="c174e-127">id</span></span>|<span data-ttu-id="c174e-128">string</span><span class="sxs-lookup"><span data-stu-id="c174e-128">string</span></span>| <span data-ttu-id="c174e-129">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="c174e-129">Read-only</span></span>|
|<span data-ttu-id="c174e-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c174e-130">ipAddress</span></span>|<span data-ttu-id="c174e-131">string</span><span class="sxs-lookup"><span data-stu-id="c174e-131">string</span></span>| <span data-ttu-id="c174e-132">2番目のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="c174e-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="c174e-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="c174e-133">isAtypicalLocation</span></span>|<span data-ttu-id="c174e-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="c174e-134">boolean</span></span>| <span data-ttu-id="c174e-135">ユーザーのいずれかの場所が例外的である場合</span><span class="sxs-lookup"><span data-stu-id="c174e-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="c174e-136">location</span><span class="sxs-lookup"><span data-stu-id="c174e-136">location</span></span>|<span data-ttu-id="c174e-137">string</span><span class="sxs-lookup"><span data-stu-id="c174e-137">string</span></span>| <span data-ttu-id="c174e-138">2番目のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="c174e-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="c174e-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="c174e-139">previousIPAddress</span></span>|<span data-ttu-id="c174e-140">string</span><span class="sxs-lookup"><span data-stu-id="c174e-140">string</span></span>| <span data-ttu-id="c174e-141">最初のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="c174e-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="c174e-142">previousLocation</span><span class="sxs-lookup"><span data-stu-id="c174e-142">previousLocation</span></span>|<span data-ttu-id="c174e-143">string</span><span class="sxs-lookup"><span data-stu-id="c174e-143">string</span></span>| <span data-ttu-id="c174e-144">最初のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="c174e-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="c174e-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="c174e-145">previousSigninDateTime</span></span>|<span data-ttu-id="c174e-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c174e-146">dateTimeOffset</span></span>| <span data-ttu-id="c174e-147">最初のサインインの日付と時刻</span><span class="sxs-lookup"><span data-stu-id="c174e-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="c174e-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c174e-148">riskEventDateTime</span></span>|<span data-ttu-id="c174e-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c174e-149">dateTimeOffset</span></span>| <span data-ttu-id="c174e-150">2番目のサインインの日付と時刻</span><span class="sxs-lookup"><span data-stu-id="c174e-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="c174e-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c174e-151">riskEventStatus</span></span>|<span data-ttu-id="c174e-152">string</span><span class="sxs-lookup"><span data-stu-id="c174e-152">string</span></span>| <span data-ttu-id="c174e-153">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="c174e-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c174e-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c174e-154">riskLevel</span></span>|<span data-ttu-id="c174e-155">string</span><span class="sxs-lookup"><span data-stu-id="c174e-155">string</span></span>| <span data-ttu-id="c174e-156">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c174e-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c174e-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c174e-157">riskEventType</span></span>|<span data-ttu-id="c174e-158">string</span><span class="sxs-lookup"><span data-stu-id="c174e-158">string</span></span>| <span data-ttu-id="c174e-159">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="c174e-159">The type of risk</span></span>|
|<span data-ttu-id="c174e-160">userAgent</span><span class="sxs-lookup"><span data-stu-id="c174e-160">userAgent</span></span>|<span data-ttu-id="c174e-161">string</span><span class="sxs-lookup"><span data-stu-id="c174e-161">string</span></span>| <span data-ttu-id="c174e-162">ブラウザーのユーザーエージェント文字列</span><span class="sxs-lookup"><span data-stu-id="c174e-162">The browser's user agent string</span></span>|
|<span data-ttu-id="c174e-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c174e-163">userDisplayName</span></span>|<span data-ttu-id="c174e-164">string</span><span class="sxs-lookup"><span data-stu-id="c174e-164">string</span></span>| <span data-ttu-id="c174e-165">リスクのあるユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="c174e-165">The name of the user at risk</span></span>|
|<span data-ttu-id="c174e-166">userId</span><span class="sxs-lookup"><span data-stu-id="c174e-166">userId</span></span>|<span data-ttu-id="c174e-167">string</span><span class="sxs-lookup"><span data-stu-id="c174e-167">string</span></span>| <span data-ttu-id="c174e-168">リスクがあるユーザーの id</span><span class="sxs-lookup"><span data-stu-id="c174e-168">The id of the user at risk</span></span>|
|<span data-ttu-id="c174e-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c174e-169">userPrincipalName</span></span>|<span data-ttu-id="c174e-170">string</span><span class="sxs-lookup"><span data-stu-id="c174e-170">string</span></span>| <span data-ttu-id="c174e-171">リスクがあるユーザーのユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="c174e-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c174e-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c174e-172">Relationships</span></span>
| <span data-ttu-id="c174e-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c174e-173">Relationship</span></span> | <span data-ttu-id="c174e-174">型</span><span class="sxs-lookup"><span data-stu-id="c174e-174">Type</span></span>   |<span data-ttu-id="c174e-175">説明</span><span class="sxs-lookup"><span data-stu-id="c174e-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c174e-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c174e-176">impactedUser</span></span>|[<span data-ttu-id="c174e-177">ユーザー</span><span class="sxs-lookup"><span data-stu-id="c174e-177">user</span></span>](user.md)| <span data-ttu-id="c174e-p102">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="c174e-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c174e-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c174e-180">JSON representation</span></span>

<span data-ttu-id="c174e-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c174e-181">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
