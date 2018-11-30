---
title: leakedCredentialsRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護野生のアカウントの資格情報が検出された場所で検出されたリスク イベントです。 リスク イベントの詳細については、Azure AD のアイデンティティ保護のマニュアルを参照しています。
ms.openlocfilehash: 2404564726c3ca7ee1f577b3d81daaa339941406
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072816"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="e7102-104">leakedCredentialsRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7102-104">leakedCredentialsRiskEvent resource type</span></span>

> <span data-ttu-id="e7102-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e7102-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7102-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7102-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7102-107">[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)野生のアカウントの資格情報が検出された場所で検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="e7102-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="e7102-108">リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="e7102-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="e7102-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7102-109">Methods</span></span>

| <span data-ttu-id="e7102-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7102-110">Method</span></span>           | <span data-ttu-id="e7102-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e7102-111">Return Type</span></span>    |<span data-ttu-id="e7102-112">説明</span><span class="sxs-lookup"><span data-stu-id="e7102-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7102-113">LeakedCredentialsRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7102-113">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="e7102-114">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e7102-114">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="e7102-115">LeakedCredentialsRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7102-115">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e7102-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7102-116">Properties</span></span>
| <span data-ttu-id="e7102-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7102-117">Property</span></span>     | <span data-ttu-id="e7102-118">型</span><span class="sxs-lookup"><span data-stu-id="e7102-118">Type</span></span>   |<span data-ttu-id="e7102-119">説明</span><span class="sxs-lookup"><span data-stu-id="e7102-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7102-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7102-120">closedDateTime</span></span>|<span data-ttu-id="e7102-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7102-121">dateTimeOffset</span></span>| <span data-ttu-id="e7102-122">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="e7102-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e7102-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7102-123">createdDateTime</span></span>|<span data-ttu-id="e7102-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7102-124">dateTimeOffset</span></span>| <span data-ttu-id="e7102-125">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="e7102-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="e7102-126">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="e7102-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e7102-127">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="e7102-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e7102-128">ID</span><span class="sxs-lookup"><span data-stu-id="e7102-128">id</span></span>|<span data-ttu-id="e7102-129">文字列</span><span class="sxs-lookup"><span data-stu-id="e7102-129">string</span></span>| <span data-ttu-id="e7102-130">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="e7102-130">Read-only</span></span>|
|<span data-ttu-id="e7102-131">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="e7102-131">riskEventDateTime</span></span>|<span data-ttu-id="e7102-132">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7102-132">dateTimeOffset</span></span>| <span data-ttu-id="e7102-133">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="e7102-133">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="e7102-134">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="e7102-134">riskEventStatus</span></span>|<span data-ttu-id="e7102-135">文字列</span><span class="sxs-lookup"><span data-stu-id="e7102-135">string</span></span>| <span data-ttu-id="e7102-136">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="e7102-136">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e7102-137">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e7102-137">riskLevel</span></span>|<span data-ttu-id="e7102-138">文字列</span><span class="sxs-lookup"><span data-stu-id="e7102-138">string</span></span>| <span data-ttu-id="e7102-139">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e7102-139">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e7102-140">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e7102-140">riskEventType</span></span>|<span data-ttu-id="e7102-141">文字列</span><span class="sxs-lookup"><span data-stu-id="e7102-141">string</span></span>| <span data-ttu-id="e7102-142">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="e7102-142">The type of risk</span></span>|
|<span data-ttu-id="e7102-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e7102-143">userDisplayName</span></span>|<span data-ttu-id="e7102-144">文字列</span><span class="sxs-lookup"><span data-stu-id="e7102-144">string</span></span>| <span data-ttu-id="e7102-145">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="e7102-145">The name of the user at risk</span></span>|
|<span data-ttu-id="e7102-146">userId</span><span class="sxs-lookup"><span data-stu-id="e7102-146">userId</span></span>|<span data-ttu-id="e7102-147">文字列</span><span class="sxs-lookup"><span data-stu-id="e7102-147">string</span></span>| <span data-ttu-id="e7102-148">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="e7102-148">The id of the user at risk</span></span>|
|<span data-ttu-id="e7102-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e7102-149">userPrincipalName</span></span>|<span data-ttu-id="e7102-150">文字列</span><span class="sxs-lookup"><span data-stu-id="e7102-150">string</span></span>| <span data-ttu-id="e7102-151">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="e7102-151">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7102-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7102-152">Relationships</span></span>
| <span data-ttu-id="e7102-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7102-153">Relationship</span></span> | <span data-ttu-id="e7102-154">型</span><span class="sxs-lookup"><span data-stu-id="e7102-154">Type</span></span>   |<span data-ttu-id="e7102-155">説明</span><span class="sxs-lookup"><span data-stu-id="e7102-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7102-156">impactedUser</span><span class="sxs-lookup"><span data-stu-id="e7102-156">impactedUser</span></span>|[<span data-ttu-id="e7102-157">user</span><span class="sxs-lookup"><span data-stu-id="e7102-157">user</span></span>](user.md)| <span data-ttu-id="e7102-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e7102-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7102-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7102-160">JSON representation</span></span>

<span data-ttu-id="e7102-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7102-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
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
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->