---
title: unfamiliarLocationRiskEvent リソースの種類
description: Azure Active Directory id 保護によって検出された、そのユーザーの新しい場所からアカウントのサインイン試行が行われたリスクイベント。 リスクイベントに関する詳細な情報については、「Azure AD Identity Protection」のドキュメントを参照してください。
localization_priority: Normal
ms.openlocfilehash: 984f11f7e47a251d49acd315d29504216b7995f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345480"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="c8807-104">unfamiliarLocationRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8807-104">unfamiliarLocationRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8807-105">[Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出された、そのユーザーの新しい場所からアカウントのサインイン試行が行われたリスクイベント。</span><span class="sxs-lookup"><span data-stu-id="c8807-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="c8807-106">リスクイベントに関する詳細な情報については、「 [Azure AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8807-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="c8807-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c8807-107">Methods</span></span>

| <span data-ttu-id="c8807-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c8807-108">Method</span></span>           | <span data-ttu-id="c8807-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c8807-109">Return Type</span></span>    |<span data-ttu-id="c8807-110">説明</span><span class="sxs-lookup"><span data-stu-id="c8807-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c8807-111">unfamiliarLocationRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="c8807-111">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="c8807-112">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c8807-112">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="c8807-113">unfamiliarLocationRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c8807-113">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8807-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8807-114">Properties</span></span>
| <span data-ttu-id="c8807-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8807-115">Property</span></span>     | <span data-ttu-id="c8807-116">型</span><span class="sxs-lookup"><span data-stu-id="c8807-116">Type</span></span>   |<span data-ttu-id="c8807-117">説明</span><span class="sxs-lookup"><span data-stu-id="c8807-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8807-118">closeddatetime</span><span class="sxs-lookup"><span data-stu-id="c8807-118">closedDateTime</span></span>|<span data-ttu-id="c8807-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8807-119">dateTimeOffset</span></span>| <span data-ttu-id="c8807-120">リスクイベントが終了した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="c8807-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c8807-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8807-121">createdDateTime</span></span>|<span data-ttu-id="c8807-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8807-122">dateTimeOffset</span></span>| <span data-ttu-id="c8807-123">リスクイベントが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c8807-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="c8807-124">これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。</span><span class="sxs-lookup"><span data-stu-id="c8807-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c8807-125">これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="c8807-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c8807-126">id</span><span class="sxs-lookup"><span data-stu-id="c8807-126">id</span></span>|<span data-ttu-id="c8807-127">文字列</span><span class="sxs-lookup"><span data-stu-id="c8807-127">string</span></span>| <span data-ttu-id="c8807-128">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="c8807-128">Read-only</span></span>|
|<span data-ttu-id="c8807-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c8807-129">ipAddress</span></span>|<span data-ttu-id="c8807-130">string</span><span class="sxs-lookup"><span data-stu-id="c8807-130">string</span></span>| <span data-ttu-id="c8807-131">サインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="c8807-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="c8807-132">location</span><span class="sxs-lookup"><span data-stu-id="c8807-132">location</span></span>|<span data-ttu-id="c8807-133">string</span><span class="sxs-lookup"><span data-stu-id="c8807-133">string</span></span>| <span data-ttu-id="c8807-134">サインインの IP アドレスに関連付けられている場所</span><span class="sxs-lookup"><span data-stu-id="c8807-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="c8807-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c8807-135">riskEventDateTime</span></span>|<span data-ttu-id="c8807-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8807-136">dateTimeOffset</span></span>| <span data-ttu-id="c8807-137">リスクイベントが発生した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="c8807-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c8807-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c8807-138">riskEventStatus</span></span>|<span data-ttu-id="c8807-139">string</span><span class="sxs-lookup"><span data-stu-id="c8807-139">string</span></span>| <span data-ttu-id="c8807-140">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="c8807-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c8807-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c8807-141">riskLevel</span></span>|<span data-ttu-id="c8807-142">string</span><span class="sxs-lookup"><span data-stu-id="c8807-142">string</span></span>| <span data-ttu-id="c8807-143">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c8807-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c8807-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c8807-144">riskEventType</span></span>|<span data-ttu-id="c8807-145">string</span><span class="sxs-lookup"><span data-stu-id="c8807-145">string</span></span>| <span data-ttu-id="c8807-146">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="c8807-146">The type of risk</span></span>|
|<span data-ttu-id="c8807-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c8807-147">userDisplayName</span></span>|<span data-ttu-id="c8807-148">string</span><span class="sxs-lookup"><span data-stu-id="c8807-148">string</span></span>| <span data-ttu-id="c8807-149">リスクのあるユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="c8807-149">The name of the user at risk</span></span>|
|<span data-ttu-id="c8807-150">userId</span><span class="sxs-lookup"><span data-stu-id="c8807-150">userId</span></span>|<span data-ttu-id="c8807-151">string</span><span class="sxs-lookup"><span data-stu-id="c8807-151">string</span></span>| <span data-ttu-id="c8807-152">リスクがあるユーザーの id</span><span class="sxs-lookup"><span data-stu-id="c8807-152">The id of the user at risk</span></span>|
|<span data-ttu-id="c8807-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c8807-153">userPrincipalName</span></span>|<span data-ttu-id="c8807-154">string</span><span class="sxs-lookup"><span data-stu-id="c8807-154">string</span></span>| <span data-ttu-id="c8807-155">リスクがあるユーザーのユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="c8807-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8807-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8807-156">Relationships</span></span>
| <span data-ttu-id="c8807-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8807-157">Relationship</span></span> | <span data-ttu-id="c8807-158">型</span><span class="sxs-lookup"><span data-stu-id="c8807-158">Type</span></span>   |<span data-ttu-id="c8807-159">説明</span><span class="sxs-lookup"><span data-stu-id="c8807-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8807-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c8807-160">impactedUser</span></span>|[<span data-ttu-id="c8807-161">user</span><span class="sxs-lookup"><span data-stu-id="c8807-161">user</span></span>](user.md)| <span data-ttu-id="c8807-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="c8807-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8807-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8807-164">JSON representation</span></span>

<span data-ttu-id="c8807-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8807-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.locatedRiskEvent",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
