---
title: impossibleTravelRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護、ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、に関する該当の記号の完全な情報の間の期間内の場所の間を移動することはできませんが検出されたリスク イベントリスク イベントは、Azure AD のアイデンティティ保護のマニュアルを参照しています。
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529384"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="69c5f-103">impossibleTravelRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69c5f-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69c5f-104">[Azure Active Directory アイデンティティの保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、記号再起動の完了の間の期間内の場所の間を移動することはできませんが検出されたリスク イベント[Azure AD のアイデンティティ保護マニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)のリスクについての情報が見つかります。</span><span class="sxs-lookup"><span data-stu-id="69c5f-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="69c5f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="69c5f-105">Methods</span></span>

| <span data-ttu-id="69c5f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="69c5f-106">Method</span></span>           | <span data-ttu-id="69c5f-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="69c5f-107">Return Type</span></span>    |<span data-ttu-id="69c5f-108">説明</span><span class="sxs-lookup"><span data-stu-id="69c5f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69c5f-109">ImpossibleTravelRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="69c5f-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="69c5f-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69c5f-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="69c5f-111">ImpossibleTravelRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69c5f-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69c5f-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69c5f-112">Properties</span></span>
| <span data-ttu-id="69c5f-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69c5f-113">Property</span></span>     | <span data-ttu-id="69c5f-114">型</span><span class="sxs-lookup"><span data-stu-id="69c5f-114">Type</span></span>   |<span data-ttu-id="69c5f-115">説明</span><span class="sxs-lookup"><span data-stu-id="69c5f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69c5f-116">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="69c5f-116">closedDateTime</span></span>|<span data-ttu-id="69c5f-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c5f-117">dateTimeOffset</span></span>| <span data-ttu-id="69c5f-118">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="69c5f-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="69c5f-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69c5f-119">createdDateTime</span></span>|<span data-ttu-id="69c5f-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c5f-120">dateTimeOffset</span></span>| <span data-ttu-id="69c5f-121">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="69c5f-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="69c5f-122">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="69c5f-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="69c5f-123">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="69c5f-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="69c5f-124">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="69c5f-124">deviceInformation</span></span>|<span data-ttu-id="69c5f-125">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-125">string</span></span>| <span data-ttu-id="69c5f-126">デバイスに関する情報</span><span class="sxs-lookup"><span data-stu-id="69c5f-126">Information about the device</span></span>|
|<span data-ttu-id="69c5f-127">id</span><span class="sxs-lookup"><span data-stu-id="69c5f-127">id</span></span>|<span data-ttu-id="69c5f-128">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-128">string</span></span>| <span data-ttu-id="69c5f-129">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="69c5f-129">Read-only</span></span>|
|<span data-ttu-id="69c5f-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="69c5f-130">ipAddress</span></span>|<span data-ttu-id="69c5f-131">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-131">string</span></span>| <span data-ttu-id="69c5f-132">2 つ目のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="69c5f-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="69c5f-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="69c5f-133">isAtypicalLocation</span></span>|<span data-ttu-id="69c5f-134">boolean</span><span class="sxs-lookup"><span data-stu-id="69c5f-134">boolean</span></span>| <span data-ttu-id="69c5f-135">ユーザーの典型的な場所のいずれかの場合</span><span class="sxs-lookup"><span data-stu-id="69c5f-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="69c5f-136">location</span><span class="sxs-lookup"><span data-stu-id="69c5f-136">location</span></span>|<span data-ttu-id="69c5f-137">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-137">string</span></span>| <span data-ttu-id="69c5f-138">2 つ目のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="69c5f-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="69c5f-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="69c5f-139">previousIPAddress</span></span>|<span data-ttu-id="69c5f-140">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-140">string</span></span>| <span data-ttu-id="69c5f-141">最初のサインインの IP アドレス</span><span class="sxs-lookup"><span data-stu-id="69c5f-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="69c5f-142">PreviousLocation</span><span class="sxs-lookup"><span data-stu-id="69c5f-142">previousLocation</span></span>|<span data-ttu-id="69c5f-143">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-143">string</span></span>| <span data-ttu-id="69c5f-144">最初のサインインの IP アドレスに接続されている場所</span><span class="sxs-lookup"><span data-stu-id="69c5f-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="69c5f-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="69c5f-145">previousSigninDateTime</span></span>|<span data-ttu-id="69c5f-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c5f-146">dateTimeOffset</span></span>| <span data-ttu-id="69c5f-147">日付と時刻の最初のサインイン</span><span class="sxs-lookup"><span data-stu-id="69c5f-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="69c5f-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="69c5f-148">riskEventDateTime</span></span>|<span data-ttu-id="69c5f-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c5f-149">dateTimeOffset</span></span>| <span data-ttu-id="69c5f-150">日付と時刻の 2 つ目のサインイン</span><span class="sxs-lookup"><span data-stu-id="69c5f-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="69c5f-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="69c5f-151">riskEventStatus</span></span>|<span data-ttu-id="69c5f-152">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-152">string</span></span>| <span data-ttu-id="69c5f-153">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="69c5f-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="69c5f-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="69c5f-154">riskLevel</span></span>|<span data-ttu-id="69c5f-155">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-155">string</span></span>| <span data-ttu-id="69c5f-156">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="69c5f-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="69c5f-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="69c5f-157">riskEventType</span></span>|<span data-ttu-id="69c5f-158">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-158">string</span></span>| <span data-ttu-id="69c5f-159">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="69c5f-159">The type of risk</span></span>|
|<span data-ttu-id="69c5f-160">UserAgent</span><span class="sxs-lookup"><span data-stu-id="69c5f-160">userAgent</span></span>|<span data-ttu-id="69c5f-161">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-161">string</span></span>| <span data-ttu-id="69c5f-162">ブラウザーのユーザー エージェント文字列</span><span class="sxs-lookup"><span data-stu-id="69c5f-162">The browser's user agent string</span></span>|
|<span data-ttu-id="69c5f-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="69c5f-163">userDisplayName</span></span>|<span data-ttu-id="69c5f-164">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-164">string</span></span>| <span data-ttu-id="69c5f-165">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="69c5f-165">The name of the user at risk</span></span>|
|<span data-ttu-id="69c5f-166">userId</span><span class="sxs-lookup"><span data-stu-id="69c5f-166">userId</span></span>|<span data-ttu-id="69c5f-167">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-167">string</span></span>| <span data-ttu-id="69c5f-168">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="69c5f-168">The id of the user at risk</span></span>|
|<span data-ttu-id="69c5f-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="69c5f-169">userPrincipalName</span></span>|<span data-ttu-id="69c5f-170">string</span><span class="sxs-lookup"><span data-stu-id="69c5f-170">string</span></span>| <span data-ttu-id="69c5f-171">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="69c5f-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="69c5f-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="69c5f-172">Relationships</span></span>
| <span data-ttu-id="69c5f-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="69c5f-173">Relationship</span></span> | <span data-ttu-id="69c5f-174">型</span><span class="sxs-lookup"><span data-stu-id="69c5f-174">Type</span></span>   |<span data-ttu-id="69c5f-175">説明</span><span class="sxs-lookup"><span data-stu-id="69c5f-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69c5f-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="69c5f-176">impactedUser</span></span>|[<span data-ttu-id="69c5f-177">user</span><span class="sxs-lookup"><span data-stu-id="69c5f-177">user</span></span>](user.md)| <span data-ttu-id="69c5f-p102">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="69c5f-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69c5f-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69c5f-180">JSON representation</span></span>

<span data-ttu-id="69c5f-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="69c5f-181">Here is a JSON representation of the resource.</span></span>

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
