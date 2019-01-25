---
title: anonymousIpRiskEvent リソースの種類
description: Azure Active Directory Id 保護場所、アカウントでサインインしようとすると匿名に表示される IP アドレスからによって検出されたリスク イベントです。 リスク イベントの詳細については、Azure AD のアイデンティティ保護のマニュアルを参照しています。
localization_priority: Normal
ms.openlocfilehash: 5f428a99466e67dfbbe4ef9b4ebe0006b56f99e9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519767"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="3f907-104">anonymousIpRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3f907-104">anonymousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f907-105">場所、アカウントでサインインしようとすると匿名に表示される IP アドレスから[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="3f907-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="3f907-106">リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="3f907-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="3f907-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f907-107">Methods</span></span>

| <span data-ttu-id="3f907-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f907-108">Method</span></span>           | <span data-ttu-id="3f907-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3f907-109">Return Type</span></span>    |<span data-ttu-id="3f907-110">説明</span><span class="sxs-lookup"><span data-stu-id="3f907-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f907-111">AnonymousIpRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="3f907-111">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="3f907-112">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="3f907-112">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="3f907-113">AnonymousIpRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f907-113">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f907-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f907-114">Properties</span></span>
| <span data-ttu-id="3f907-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f907-115">Property</span></span>     | <span data-ttu-id="3f907-116">型</span><span class="sxs-lookup"><span data-stu-id="3f907-116">Type</span></span>   |<span data-ttu-id="3f907-117">説明</span><span class="sxs-lookup"><span data-stu-id="3f907-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f907-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f907-118">closedDateTime</span></span>|<span data-ttu-id="3f907-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f907-119">dateTimeOffset</span></span>| <span data-ttu-id="3f907-120">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="3f907-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="3f907-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f907-121">createdDateTime</span></span>|<span data-ttu-id="3f907-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f907-122">dateTimeOffset</span></span>| <span data-ttu-id="3f907-123">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="3f907-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="3f907-124">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="3f907-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="3f907-125">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="3f907-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="3f907-126">id</span><span class="sxs-lookup"><span data-stu-id="3f907-126">id</span></span>|<span data-ttu-id="3f907-127">string</span><span class="sxs-lookup"><span data-stu-id="3f907-127">string</span></span>| <span data-ttu-id="3f907-128">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="3f907-128">Read-only</span></span>|
|<span data-ttu-id="3f907-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3f907-129">ipAddress</span></span>|<span data-ttu-id="3f907-130">string</span><span class="sxs-lookup"><span data-stu-id="3f907-130">string</span></span>| <span data-ttu-id="3f907-131">サインイン用の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="3f907-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="3f907-132">location</span><span class="sxs-lookup"><span data-stu-id="3f907-132">location</span></span>|<span data-ttu-id="3f907-133">string</span><span class="sxs-lookup"><span data-stu-id="3f907-133">string</span></span>| <span data-ttu-id="3f907-134">サインイン用の IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="3f907-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="3f907-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="3f907-135">riskEventDateTime</span></span>|<span data-ttu-id="3f907-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f907-136">dateTimeOffset</span></span>| <span data-ttu-id="3f907-137">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="3f907-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="3f907-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="3f907-138">riskEventStatus</span></span>|<span data-ttu-id="3f907-139">string</span><span class="sxs-lookup"><span data-stu-id="3f907-139">string</span></span>| <span data-ttu-id="3f907-140">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="3f907-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="3f907-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3f907-141">riskLevel</span></span>|<span data-ttu-id="3f907-142">string</span><span class="sxs-lookup"><span data-stu-id="3f907-142">string</span></span>| <span data-ttu-id="3f907-143">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="3f907-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="3f907-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="3f907-144">riskEventType</span></span>|<span data-ttu-id="3f907-145">string</span><span class="sxs-lookup"><span data-stu-id="3f907-145">string</span></span>| <span data-ttu-id="3f907-146">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="3f907-146">The type of risk</span></span>|
|<span data-ttu-id="3f907-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3f907-147">userDisplayName</span></span>|<span data-ttu-id="3f907-148">string</span><span class="sxs-lookup"><span data-stu-id="3f907-148">string</span></span>| <span data-ttu-id="3f907-149">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="3f907-149">The name of the user at risk</span></span>|
|<span data-ttu-id="3f907-150">userId</span><span class="sxs-lookup"><span data-stu-id="3f907-150">userId</span></span>|<span data-ttu-id="3f907-151">string</span><span class="sxs-lookup"><span data-stu-id="3f907-151">string</span></span>| <span data-ttu-id="3f907-152">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="3f907-152">The id of the user at risk</span></span>|
|<span data-ttu-id="3f907-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3f907-153">userPrincipalName</span></span>|<span data-ttu-id="3f907-154">string</span><span class="sxs-lookup"><span data-stu-id="3f907-154">string</span></span>| <span data-ttu-id="3f907-155">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="3f907-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f907-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3f907-156">Relationships</span></span>
| <span data-ttu-id="3f907-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3f907-157">Relationship</span></span> | <span data-ttu-id="3f907-158">型</span><span class="sxs-lookup"><span data-stu-id="3f907-158">Type</span></span>   |<span data-ttu-id="3f907-159">説明</span><span class="sxs-lookup"><span data-stu-id="3f907-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f907-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="3f907-160">impactedUser</span></span>|[<span data-ttu-id="3f907-161">user</span><span class="sxs-lookup"><span data-stu-id="3f907-161">user</span></span>](user.md)| <span data-ttu-id="3f907-p104">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="3f907-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f907-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3f907-164">JSON representation</span></span>

<span data-ttu-id="3f907-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3f907-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/anonymousipriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
