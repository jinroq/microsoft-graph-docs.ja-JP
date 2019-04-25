---
title: locatedRiskEvent リソースの種類
description: 場所データに基づく Azure Active Directory id 保護によって検出されたリスクイベント。 存在するリスクイベントの種類は次のとおりです。
localization_priority: Normal
ms.openlocfilehash: 20fe76099c511483144b42e33fc260910debb5ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578153"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="450df-104">locatedRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="450df-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="450df-105">場所データに基づく[Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスクイベント。</span><span class="sxs-lookup"><span data-stu-id="450df-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="450df-106">存在するリスクイベントの種類は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="450df-106">Located risk event types include:</span></span>
* [<span data-ttu-id="450df-107">匿名 IP アドレスからのサインイン</span><span class="sxs-lookup"><span data-stu-id="450df-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="450df-108">マルウェアに感染したデバイスからのサインイン</span><span class="sxs-lookup"><span data-stu-id="450df-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="450df-109">例外的でない場所への移動は不可能</span><span class="sxs-lookup"><span data-stu-id="450df-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="450df-110">疑わしい IP アドレスからのサインイン</span><span class="sxs-lookup"><span data-stu-id="450df-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="450df-111">[見慣れない場所からのサインイン](unfamiliarlocationriskevent.md)リスクイベントに関する詳細な情報については、「 [Azure AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="450df-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="450df-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="450df-112">Methods</span></span>

| <span data-ttu-id="450df-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="450df-113">Method</span></span>           | <span data-ttu-id="450df-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="450df-114">Return Type</span></span>    |<span data-ttu-id="450df-115">説明</span><span class="sxs-lookup"><span data-stu-id="450df-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="450df-116">locatedRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="450df-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="450df-117">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="450df-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="450df-118">locatedRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="450df-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="450df-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="450df-119">Properties</span></span>
| <span data-ttu-id="450df-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="450df-120">Property</span></span>     | <span data-ttu-id="450df-121">型</span><span class="sxs-lookup"><span data-stu-id="450df-121">Type</span></span>   |<span data-ttu-id="450df-122">説明</span><span class="sxs-lookup"><span data-stu-id="450df-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="450df-123">closeddatetime</span><span class="sxs-lookup"><span data-stu-id="450df-123">closedDateTime</span></span>|<span data-ttu-id="450df-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="450df-124">dateTimeOffset</span></span>| <span data-ttu-id="450df-125">リスクイベントが終了した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="450df-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="450df-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="450df-126">createdDateTime</span></span>|<span data-ttu-id="450df-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="450df-127">dateTimeOffset</span></span>| <span data-ttu-id="450df-128">リスクイベントが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="450df-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="450df-129">これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。</span><span class="sxs-lookup"><span data-stu-id="450df-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="450df-130">これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="450df-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="450df-131">id</span><span class="sxs-lookup"><span data-stu-id="450df-131">id</span></span>|<span data-ttu-id="450df-132">string</span><span class="sxs-lookup"><span data-stu-id="450df-132">string</span></span>| <span data-ttu-id="450df-133">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="450df-133">Read-only</span></span>|
|<span data-ttu-id="450df-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="450df-134">ipAddress</span></span>|<span data-ttu-id="450df-135">string</span><span class="sxs-lookup"><span data-stu-id="450df-135">string</span></span>| <span data-ttu-id="450df-136">サインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="450df-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="450df-137">location</span><span class="sxs-lookup"><span data-stu-id="450df-137">location</span></span>|<span data-ttu-id="450df-138">string</span><span class="sxs-lookup"><span data-stu-id="450df-138">string</span></span>| <span data-ttu-id="450df-139">サインインの IP アドレスに関連付けられている場所</span><span class="sxs-lookup"><span data-stu-id="450df-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="450df-140">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="450df-140">riskEventDateTime</span></span>|<span data-ttu-id="450df-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="450df-141">dateTimeOffset</span></span>| <span data-ttu-id="450df-142">リスクイベントが発生した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="450df-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="450df-143">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="450df-143">riskEventStatus</span></span>|<span data-ttu-id="450df-144">string</span><span class="sxs-lookup"><span data-stu-id="450df-144">string</span></span>| <span data-ttu-id="450df-145">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="450df-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="450df-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="450df-146">riskLevel</span></span>|<span data-ttu-id="450df-147">string</span><span class="sxs-lookup"><span data-stu-id="450df-147">string</span></span>| <span data-ttu-id="450df-148">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="450df-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="450df-149">riskEventType</span><span class="sxs-lookup"><span data-stu-id="450df-149">riskEventType</span></span>|<span data-ttu-id="450df-150">string</span><span class="sxs-lookup"><span data-stu-id="450df-150">string</span></span>| <span data-ttu-id="450df-151">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="450df-151">The type of risk</span></span>|
|<span data-ttu-id="450df-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="450df-152">userDisplayName</span></span>|<span data-ttu-id="450df-153">string</span><span class="sxs-lookup"><span data-stu-id="450df-153">string</span></span>| <span data-ttu-id="450df-154">リスクのあるユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="450df-154">The name of the user at risk</span></span>|
|<span data-ttu-id="450df-155">userId</span><span class="sxs-lookup"><span data-stu-id="450df-155">userId</span></span>|<span data-ttu-id="450df-156">string</span><span class="sxs-lookup"><span data-stu-id="450df-156">string</span></span>| <span data-ttu-id="450df-157">リスクがあるユーザーの id</span><span class="sxs-lookup"><span data-stu-id="450df-157">The id of the user at risk</span></span>|
|<span data-ttu-id="450df-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="450df-158">userPrincipalName</span></span>|<span data-ttu-id="450df-159">string</span><span class="sxs-lookup"><span data-stu-id="450df-159">string</span></span>| <span data-ttu-id="450df-160">リスクがあるユーザーのユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="450df-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="450df-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="450df-161">Relationships</span></span>
| <span data-ttu-id="450df-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="450df-162">Relationship</span></span> | <span data-ttu-id="450df-163">型</span><span class="sxs-lookup"><span data-stu-id="450df-163">Type</span></span>   |<span data-ttu-id="450df-164">説明</span><span class="sxs-lookup"><span data-stu-id="450df-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="450df-165">impactedUser</span><span class="sxs-lookup"><span data-stu-id="450df-165">impactedUser</span></span>|[<span data-ttu-id="450df-166">ユーザー</span><span class="sxs-lookup"><span data-stu-id="450df-166">user</span></span>](user.md)| <span data-ttu-id="450df-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="450df-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="450df-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="450df-169">JSON representation</span></span>

<span data-ttu-id="450df-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="450df-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locatedRiskEvent"
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locatedriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
