---
title: privilegedRoleSettings リソースの種類
description: 特権を持つロールの設定を表します。
localization_priority: Normal
ms.openlocfilehash: 971c48ce3ecdd2a219a111f3a11884377e20430c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842743"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="51dd8-103">privilegedRoleSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51dd8-103">privilegedRoleSettings resource type</span></span>

> <span data-ttu-id="51dd8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51dd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51dd8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51dd8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51dd8-106">特権を持つロールの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="51dd8-106">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="51dd8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="51dd8-107">Methods</span></span>

| <span data-ttu-id="51dd8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="51dd8-108">Method</span></span>           | <span data-ttu-id="51dd8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="51dd8-109">Return Type</span></span>    |<span data-ttu-id="51dd8-110">説明</span><span class="sxs-lookup"><span data-stu-id="51dd8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51dd8-111">PrivilegedRoleSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="51dd8-111">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="51dd8-112">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="51dd8-112">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="51dd8-113">PrivilegedRoleSettings オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51dd8-113">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="51dd8-114">PrivilegedRoleSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="51dd8-114">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="51dd8-115">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="51dd8-115">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="51dd8-116">PrivilegedRoleSettings オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="51dd8-116">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="51dd8-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51dd8-117">Properties</span></span>
| <span data-ttu-id="51dd8-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51dd8-118">Property</span></span>     | <span data-ttu-id="51dd8-119">種類</span><span class="sxs-lookup"><span data-stu-id="51dd8-119">Type</span></span>   |<span data-ttu-id="51dd8-120">説明</span><span class="sxs-lookup"><span data-stu-id="51dd8-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51dd8-121">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="51dd8-121">elevationDuration</span></span>|<span data-ttu-id="51dd8-122">duration</span><span class="sxs-lookup"><span data-stu-id="51dd8-122">duration</span></span>|<span data-ttu-id="51dd8-123">ロールが有効な場合の期間です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-123">The duration when the role is activated.</span></span>|
|<span data-ttu-id="51dd8-124">ID</span><span class="sxs-lookup"><span data-stu-id="51dd8-124">id</span></span>|<span data-ttu-id="51dd8-125">文字列</span><span class="sxs-lookup"><span data-stu-id="51dd8-125">string</span></span>| <span data-ttu-id="51dd8-126">ロールの設定の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-126">The unique identifier for the role settings.</span></span> <span data-ttu-id="51dd8-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-127">Read-only.</span></span>|
|<span data-ttu-id="51dd8-128">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="51dd8-128">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="51dd8-129">ブール</span><span class="sxs-lookup"><span data-stu-id="51dd8-129">boolean</span></span>|<span data-ttu-id="51dd8-130">**真**mfaOnElevation は、構成可能な場合です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-130">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="51dd8-131">場合は**false を指定**mfaOnElevation は構成できません。</span><span class="sxs-lookup"><span data-stu-id="51dd8-131">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="51dd8-132">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="51dd8-132">lastGlobalAdmin</span></span>|<span data-ttu-id="51dd8-133">ブール</span><span class="sxs-lookup"><span data-stu-id="51dd8-133">boolean</span></span>|<span data-ttu-id="51dd8-134">内部エラーのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="51dd8-134">Internal used only.</span></span>|
|<span data-ttu-id="51dd8-135">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="51dd8-135">maxElavationDuration</span></span>|<span data-ttu-id="51dd8-136">duration</span><span class="sxs-lookup"><span data-stu-id="51dd8-136">duration</span></span>|<span data-ttu-id="51dd8-137">アクティブ化されたロールの最大の期間です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-137">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="51dd8-138">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="51dd8-138">mfaOnElevation</span></span>|<span data-ttu-id="51dd8-139">ブール</span><span class="sxs-lookup"><span data-stu-id="51dd8-139">boolean</span></span>|<span data-ttu-id="51dd8-140">**true** MFA は、ロールをアクティブにするために必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-140">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="51dd8-141">**false**場合は、MFA は、ロールをアクティブにする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="51dd8-141">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="51dd8-142">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="51dd8-142">minElevationDuration</span></span>|<span data-ttu-id="51dd8-143">duration</span><span class="sxs-lookup"><span data-stu-id="51dd8-143">duration</span></span>|<span data-ttu-id="51dd8-144">アクティブ化されたロールの最低限の期間です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-144">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="51dd8-145">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="51dd8-145">notificationToUserOnElevation</span></span>|<span data-ttu-id="51dd8-146">ブール</span><span class="sxs-lookup"><span data-stu-id="51dd8-146">boolean</span></span>|<span data-ttu-id="51dd8-147">**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="51dd8-147">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="51dd8-148">**false**場合は、ロールがアクティブになったときに通知を送信できません。</span><span class="sxs-lookup"><span data-stu-id="51dd8-148">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="51dd8-149">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="51dd8-149">ticketingInfoOnElevation</span></span>|<span data-ttu-id="51dd8-150">ブール</span><span class="sxs-lookup"><span data-stu-id="51dd8-150">boolean</span></span>|<span data-ttu-id="51dd8-151">**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="51dd8-151">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="51dd8-152">**false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="51dd8-152">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="51dd8-153">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="51dd8-153">approvalOnElevation</span></span>|<span data-ttu-id="51dd8-154">ブール</span><span class="sxs-lookup"><span data-stu-id="51dd8-154">boolean</span></span>|<span data-ttu-id="51dd8-155">**true の**場合は、承認が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="51dd8-155">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="51dd8-156">**false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="51dd8-156">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="51dd8-157">approverIds</span><span class="sxs-lookup"><span data-stu-id="51dd8-157">approverIds</span></span>|<span data-ttu-id="51dd8-158">配列</span><span class="sxs-lookup"><span data-stu-id="51dd8-158">array</span></span>|<span data-ttu-id="51dd8-159">承認 id、ライセンス認証の必要な場合は承認の一覧です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-159">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51dd8-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51dd8-160">Relationships</span></span>
<span data-ttu-id="51dd8-161">なし</span><span class="sxs-lookup"><span data-stu-id="51dd8-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="51dd8-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51dd8-162">JSON representation</span></span>

<span data-ttu-id="51dd8-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51dd8-163">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
