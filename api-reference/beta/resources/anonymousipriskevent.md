---
title: anonymousIpRiskEvent リソースの種類
description: Azure Active Directory Id 保護によって検出された、匿名の IP アドレスからアカウントのサインインが試行されるリスクイベント。 リスクイベントに関する詳細な情報については、「Azure AD Identity Protection」のドキュメントを参照してください。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5016aac704feb35383dc34e58f3ed06657733edf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013393"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="7cdcc-104">anonymousIpRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7cdcc-104">anonymousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cdcc-105">[Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出された、匿名の IP アドレスからアカウントのサインインが試行されるリスクイベント。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="7cdcc-106">リスクイベントに関する詳細な情報については、「 [AZURE AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="7cdcc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7cdcc-107">Methods</span></span>

| <span data-ttu-id="7cdcc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7cdcc-108">Method</span></span>           | <span data-ttu-id="7cdcc-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7cdcc-109">Return Type</span></span>    |<span data-ttu-id="7cdcc-110">説明</span><span class="sxs-lookup"><span data-stu-id="7cdcc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7cdcc-111">anonymousIpRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="7cdcc-111">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="7cdcc-112">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7cdcc-112">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="7cdcc-113">AnonymousIpRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-113">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7cdcc-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cdcc-114">Properties</span></span>
| <span data-ttu-id="7cdcc-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cdcc-115">Property</span></span>     | <span data-ttu-id="7cdcc-116">型</span><span class="sxs-lookup"><span data-stu-id="7cdcc-116">Type</span></span>   |<span data-ttu-id="7cdcc-117">説明</span><span class="sxs-lookup"><span data-stu-id="7cdcc-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cdcc-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cdcc-118">closedDateTime</span></span>|<span data-ttu-id="7cdcc-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cdcc-119">dateTimeOffset</span></span>| <span data-ttu-id="7cdcc-120">リスクイベントが終了した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="7cdcc-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="7cdcc-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7cdcc-121">createdDateTime</span></span>|<span data-ttu-id="7cdcc-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cdcc-122">dateTimeOffset</span></span>| <span data-ttu-id="7cdcc-123">リスクイベントが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="7cdcc-124">これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="7cdcc-125">これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="7cdcc-126">id</span><span class="sxs-lookup"><span data-stu-id="7cdcc-126">id</span></span>|<span data-ttu-id="7cdcc-127">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-127">string</span></span>| <span data-ttu-id="7cdcc-128">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="7cdcc-128">Read-only</span></span>|
|<span data-ttu-id="7cdcc-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="7cdcc-129">ipAddress</span></span>|<span data-ttu-id="7cdcc-130">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-130">string</span></span>| <span data-ttu-id="7cdcc-131">サインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="7cdcc-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="7cdcc-132">location</span><span class="sxs-lookup"><span data-stu-id="7cdcc-132">location</span></span>|<span data-ttu-id="7cdcc-133">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-133">string</span></span>| <span data-ttu-id="7cdcc-134">サインインの IP アドレスに関連付けられている場所</span><span class="sxs-lookup"><span data-stu-id="7cdcc-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="7cdcc-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="7cdcc-135">riskEventDateTime</span></span>|<span data-ttu-id="7cdcc-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cdcc-136">dateTimeOffset</span></span>| <span data-ttu-id="7cdcc-137">リスクイベントが発生した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="7cdcc-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="7cdcc-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="7cdcc-138">riskEventStatus</span></span>|<span data-ttu-id="7cdcc-139">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-139">string</span></span>| <span data-ttu-id="7cdcc-140">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="7cdcc-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="7cdcc-141">riskLevel</span></span>|<span data-ttu-id="7cdcc-142">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-142">string</span></span>| <span data-ttu-id="7cdcc-143">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="7cdcc-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="7cdcc-144">riskEventType</span></span>|<span data-ttu-id="7cdcc-145">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-145">string</span></span>| <span data-ttu-id="7cdcc-146">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="7cdcc-146">The type of risk</span></span>|
|<span data-ttu-id="7cdcc-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7cdcc-147">userDisplayName</span></span>|<span data-ttu-id="7cdcc-148">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-148">string</span></span>| <span data-ttu-id="7cdcc-149">リスクのあるユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="7cdcc-149">The name of the user at risk</span></span>|
|<span data-ttu-id="7cdcc-150">userId</span><span class="sxs-lookup"><span data-stu-id="7cdcc-150">userId</span></span>|<span data-ttu-id="7cdcc-151">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-151">string</span></span>| <span data-ttu-id="7cdcc-152">リスクがあるユーザーの id</span><span class="sxs-lookup"><span data-stu-id="7cdcc-152">The id of the user at risk</span></span>|
|<span data-ttu-id="7cdcc-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7cdcc-153">userPrincipalName</span></span>|<span data-ttu-id="7cdcc-154">string</span><span class="sxs-lookup"><span data-stu-id="7cdcc-154">string</span></span>| <span data-ttu-id="7cdcc-155">リスクがあるユーザーのユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="7cdcc-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cdcc-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7cdcc-156">Relationships</span></span>
| <span data-ttu-id="7cdcc-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7cdcc-157">Relationship</span></span> | <span data-ttu-id="7cdcc-158">型</span><span class="sxs-lookup"><span data-stu-id="7cdcc-158">Type</span></span>   |<span data-ttu-id="7cdcc-159">説明</span><span class="sxs-lookup"><span data-stu-id="7cdcc-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cdcc-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="7cdcc-160">impactedUser</span></span>|[<span data-ttu-id="7cdcc-161">ユーザー</span><span class="sxs-lookup"><span data-stu-id="7cdcc-161">user</span></span>](user.md)| <span data-ttu-id="7cdcc-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cdcc-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7cdcc-164">JSON representation</span></span>

<span data-ttu-id="7cdcc-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7cdcc-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
