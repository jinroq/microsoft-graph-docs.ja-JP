---
title: leakedCredentialsRiskEvent リソースの種類
description: アカウントの資格情報がワイルドカードで検出された Azure Active Directory Id 保護によって検出されたリスクイベント。 リスクイベントに関する詳細な情報については、「Azure AD Identity Protection」のドキュメントを参照してください。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3c6ae090a4b9359883dfbadacb09bc3ebcc11817
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010008"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="c7640-104">leakedCredentialsRiskEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7640-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7640-105">アカウントの資格情報がワイルドカードで検出された[Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスクイベント。</span><span class="sxs-lookup"><span data-stu-id="c7640-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="c7640-106">リスクイベントに関する詳細な情報については、「 [AZURE AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7640-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="c7640-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7640-107">Methods</span></span>

| <span data-ttu-id="c7640-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7640-108">Method</span></span>           | <span data-ttu-id="c7640-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c7640-109">Return Type</span></span>    |<span data-ttu-id="c7640-110">説明</span><span class="sxs-lookup"><span data-stu-id="c7640-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7640-111">leakedCredentialsRiskEvent を取得する</span><span class="sxs-lookup"><span data-stu-id="c7640-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="c7640-112">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7640-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="c7640-113">LeakedCredentialsRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c7640-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7640-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7640-114">Properties</span></span>
| <span data-ttu-id="c7640-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7640-115">Property</span></span>     | <span data-ttu-id="c7640-116">型</span><span class="sxs-lookup"><span data-stu-id="c7640-116">Type</span></span>   |<span data-ttu-id="c7640-117">説明</span><span class="sxs-lookup"><span data-stu-id="c7640-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7640-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7640-118">closedDateTime</span></span>|<span data-ttu-id="c7640-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7640-119">dateTimeOffset</span></span>| <span data-ttu-id="c7640-120">リスクイベントが終了した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="c7640-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c7640-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7640-121">createdDateTime</span></span>|<span data-ttu-id="c7640-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7640-122">dateTimeOffset</span></span>| <span data-ttu-id="c7640-123">リスクイベントが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c7640-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="c7640-124">これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。</span><span class="sxs-lookup"><span data-stu-id="c7640-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c7640-125">これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="c7640-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c7640-126">id</span><span class="sxs-lookup"><span data-stu-id="c7640-126">id</span></span>|<span data-ttu-id="c7640-127">string</span><span class="sxs-lookup"><span data-stu-id="c7640-127">string</span></span>| <span data-ttu-id="c7640-128">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="c7640-128">Read-only</span></span>|
|<span data-ttu-id="c7640-129">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c7640-129">riskEventDateTime</span></span>|<span data-ttu-id="c7640-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7640-130">dateTimeOffset</span></span>| <span data-ttu-id="c7640-131">リスクイベントが発生した日付と時刻</span><span class="sxs-lookup"><span data-stu-id="c7640-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c7640-132">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c7640-132">riskEventStatus</span></span>|<span data-ttu-id="c7640-133">string</span><span class="sxs-lookup"><span data-stu-id="c7640-133">string</span></span>| <span data-ttu-id="c7640-134">可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。</span><span class="sxs-lookup"><span data-stu-id="c7640-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c7640-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c7640-135">riskLevel</span></span>|<span data-ttu-id="c7640-136">string</span><span class="sxs-lookup"><span data-stu-id="c7640-136">string</span></span>| <span data-ttu-id="c7640-137">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c7640-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c7640-138">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c7640-138">riskEventType</span></span>|<span data-ttu-id="c7640-139">string</span><span class="sxs-lookup"><span data-stu-id="c7640-139">string</span></span>| <span data-ttu-id="c7640-140">リスクの種類</span><span class="sxs-lookup"><span data-stu-id="c7640-140">The type of risk</span></span>|
|<span data-ttu-id="c7640-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7640-141">userDisplayName</span></span>|<span data-ttu-id="c7640-142">string</span><span class="sxs-lookup"><span data-stu-id="c7640-142">string</span></span>| <span data-ttu-id="c7640-143">リスクのあるユーザーの名前</span><span class="sxs-lookup"><span data-stu-id="c7640-143">The name of the user at risk</span></span>|
|<span data-ttu-id="c7640-144">userId</span><span class="sxs-lookup"><span data-stu-id="c7640-144">userId</span></span>|<span data-ttu-id="c7640-145">string</span><span class="sxs-lookup"><span data-stu-id="c7640-145">string</span></span>| <span data-ttu-id="c7640-146">リスクがあるユーザーの id</span><span class="sxs-lookup"><span data-stu-id="c7640-146">The id of the user at risk</span></span>|
|<span data-ttu-id="c7640-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7640-147">userPrincipalName</span></span>|<span data-ttu-id="c7640-148">string</span><span class="sxs-lookup"><span data-stu-id="c7640-148">string</span></span>| <span data-ttu-id="c7640-149">リスクがあるユーザーのユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="c7640-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7640-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7640-150">Relationships</span></span>
| <span data-ttu-id="c7640-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7640-151">Relationship</span></span> | <span data-ttu-id="c7640-152">型</span><span class="sxs-lookup"><span data-stu-id="c7640-152">Type</span></span>   |<span data-ttu-id="c7640-153">説明</span><span class="sxs-lookup"><span data-stu-id="c7640-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7640-154">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c7640-154">impactedUser</span></span>|[<span data-ttu-id="c7640-155">ユーザー</span><span class="sxs-lookup"><span data-stu-id="c7640-155">user</span></span>](user.md)| <span data-ttu-id="c7640-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="c7640-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7640-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7640-158">JSON representation</span></span>

<span data-ttu-id="c7640-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7640-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
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
  "suppressions": []
}
-->
