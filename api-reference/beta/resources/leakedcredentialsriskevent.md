---
title: leakedCredentialsRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護野生のアカウントの資格情報が検出された場所で検出されたリスク イベントです。 リスク イベントの詳細については、Azure AD のアイデンティティ保護のマニュアルを参照しています。
localization_priority: Normal
ms.openlocfilehash: 0884da08195ffa2bee38c943d27b1d25aef02e49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510989"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="ce8fa-104">leakedCredentialsRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce8fa-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce8fa-105">[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)野生のアカウントの資格情報が検出された場所で検出されたリスク イベントです。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="ce8fa-106">リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)を参照しています。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="ce8fa-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce8fa-107">Methods</span></span>

| <span data-ttu-id="ce8fa-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce8fa-108">Method</span></span>           | <span data-ttu-id="ce8fa-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce8fa-109">Return Type</span></span>    |<span data-ttu-id="ce8fa-110">説明</span><span class="sxs-lookup"><span data-stu-id="ce8fa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce8fa-111">LeakedCredentialsRiskEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="ce8fa-112">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ce8fa-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="ce8fa-113">LeakedCredentialsRiskEvent オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce8fa-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce8fa-114">Properties</span></span>
| <span data-ttu-id="ce8fa-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce8fa-115">Property</span></span>     | <span data-ttu-id="ce8fa-116">型</span><span class="sxs-lookup"><span data-stu-id="ce8fa-116">Type</span></span>   |<span data-ttu-id="ce8fa-117">説明</span><span class="sxs-lookup"><span data-stu-id="ce8fa-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce8fa-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8fa-118">closedDateTime</span></span>|<span data-ttu-id="ce8fa-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8fa-119">dateTimeOffset</span></span>| <span data-ttu-id="ce8fa-120">リスク イベントが終了したときの日時</span><span class="sxs-lookup"><span data-stu-id="ce8fa-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="ce8fa-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8fa-121">createdDateTime</span></span>|<span data-ttu-id="ce8fa-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8fa-122">dateTimeOffset</span></span>| <span data-ttu-id="ce8fa-123">日付とイベントが作成された時刻です。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="ce8fa-124">以上のリスク イベント自体の日付と時刻を常にです。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="ce8fa-125">これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="ce8fa-126">id</span><span class="sxs-lookup"><span data-stu-id="ce8fa-126">id</span></span>|<span data-ttu-id="ce8fa-127">string</span><span class="sxs-lookup"><span data-stu-id="ce8fa-127">string</span></span>| <span data-ttu-id="ce8fa-128">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="ce8fa-128">Read-only</span></span>|
|<span data-ttu-id="ce8fa-129">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8fa-129">riskEventDateTime</span></span>|<span data-ttu-id="ce8fa-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8fa-130">dateTimeOffset</span></span>| <span data-ttu-id="ce8fa-131">リスク イベントが発生したときの日時</span><span class="sxs-lookup"><span data-stu-id="ce8fa-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="ce8fa-132">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="ce8fa-132">riskEventStatus</span></span>|<span data-ttu-id="ce8fa-133">string</span><span class="sxs-lookup"><span data-stu-id="ce8fa-133">string</span></span>| <span data-ttu-id="ce8fa-134">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="ce8fa-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ce8fa-135">riskLevel</span></span>|<span data-ttu-id="ce8fa-136">string</span><span class="sxs-lookup"><span data-stu-id="ce8fa-136">string</span></span>| <span data-ttu-id="ce8fa-137">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="ce8fa-138">riskEventType</span><span class="sxs-lookup"><span data-stu-id="ce8fa-138">riskEventType</span></span>|<span data-ttu-id="ce8fa-139">string</span><span class="sxs-lookup"><span data-stu-id="ce8fa-139">string</span></span>| <span data-ttu-id="ce8fa-140">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="ce8fa-140">The type of risk</span></span>|
|<span data-ttu-id="ce8fa-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ce8fa-141">userDisplayName</span></span>|<span data-ttu-id="ce8fa-142">string</span><span class="sxs-lookup"><span data-stu-id="ce8fa-142">string</span></span>| <span data-ttu-id="ce8fa-143">リスクのユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="ce8fa-143">The name of the user at risk</span></span>|
|<span data-ttu-id="ce8fa-144">userId</span><span class="sxs-lookup"><span data-stu-id="ce8fa-144">userId</span></span>|<span data-ttu-id="ce8fa-145">string</span><span class="sxs-lookup"><span data-stu-id="ce8fa-145">string</span></span>| <span data-ttu-id="ce8fa-146">リスクのユーザーの id</span><span class="sxs-lookup"><span data-stu-id="ce8fa-146">The id of the user at risk</span></span>|
|<span data-ttu-id="ce8fa-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ce8fa-147">userPrincipalName</span></span>|<span data-ttu-id="ce8fa-148">string</span><span class="sxs-lookup"><span data-stu-id="ce8fa-148">string</span></span>| <span data-ttu-id="ce8fa-149">リスクのユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="ce8fa-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce8fa-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce8fa-150">Relationships</span></span>
| <span data-ttu-id="ce8fa-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce8fa-151">Relationship</span></span> | <span data-ttu-id="ce8fa-152">型</span><span class="sxs-lookup"><span data-stu-id="ce8fa-152">Type</span></span>   |<span data-ttu-id="ce8fa-153">説明</span><span class="sxs-lookup"><span data-stu-id="ce8fa-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce8fa-154">impactedUser</span><span class="sxs-lookup"><span data-stu-id="ce8fa-154">impactedUser</span></span>|[<span data-ttu-id="ce8fa-155">user</span><span class="sxs-lookup"><span data-stu-id="ce8fa-155">user</span></span>](user.md)| <span data-ttu-id="ce8fa-p104">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce8fa-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce8fa-158">JSON representation</span></span>

<span data-ttu-id="ce8fa-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce8fa-159">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/leakedcredentialsriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
