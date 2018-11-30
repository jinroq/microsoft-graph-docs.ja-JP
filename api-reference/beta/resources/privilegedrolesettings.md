---
title: privilegedRoleSettings リソースの種類
description: 特権を持つロールの設定を表します。
ms.openlocfilehash: 14b4919d653de80c97f06aff507c011162c3c0e4
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/30/2018
ms.locfileid: "27074559"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="40366-103">privilegedRoleSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40366-103">privilegedRoleSettings resource type</span></span>

> <span data-ttu-id="40366-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="40366-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40366-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40366-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40366-106">特権を持つロールの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="40366-106">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="40366-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="40366-107">Methods</span></span>

| <span data-ttu-id="40366-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="40366-108">Method</span></span>           | <span data-ttu-id="40366-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="40366-109">Return Type</span></span>    |<span data-ttu-id="40366-110">説明</span><span class="sxs-lookup"><span data-stu-id="40366-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40366-111">PrivilegedRoleSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="40366-111">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="40366-112">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="40366-112">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="40366-113">PrivilegedRoleSettings オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40366-113">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="40366-114">PrivilegedRoleSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="40366-114">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="40366-115">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="40366-115">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="40366-116">PrivilegedRoleSettings オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="40366-116">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="40366-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40366-117">Properties</span></span>
| <span data-ttu-id="40366-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40366-118">Property</span></span>     | <span data-ttu-id="40366-119">型</span><span class="sxs-lookup"><span data-stu-id="40366-119">Type</span></span>   |<span data-ttu-id="40366-120">説明</span><span class="sxs-lookup"><span data-stu-id="40366-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40366-121">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="40366-121">elevationDuration</span></span>|<span data-ttu-id="40366-122">duration</span><span class="sxs-lookup"><span data-stu-id="40366-122">duration</span></span>|<span data-ttu-id="40366-123">ロールが有効な場合の期間です。</span><span class="sxs-lookup"><span data-stu-id="40366-123">The duration when the role is activated.</span></span>|
|<span data-ttu-id="40366-124">ID</span><span class="sxs-lookup"><span data-stu-id="40366-124">id</span></span>|<span data-ttu-id="40366-125">文字列</span><span class="sxs-lookup"><span data-stu-id="40366-125">string</span></span>| <span data-ttu-id="40366-126">ロールの設定の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="40366-126">The unique identifier for the role settings.</span></span> <span data-ttu-id="40366-127">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="40366-127">Read-only.</span></span>|
|<span data-ttu-id="40366-128">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="40366-128">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="40366-129">ブール</span><span class="sxs-lookup"><span data-stu-id="40366-129">boolean</span></span>|<span data-ttu-id="40366-130">**真**mfaOnElevation は、構成可能な場合です。</span><span class="sxs-lookup"><span data-stu-id="40366-130">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="40366-131">場合は**false を指定**mfaOnElevation は構成できません。</span><span class="sxs-lookup"><span data-stu-id="40366-131">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="40366-132">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="40366-132">lastGlobalAdmin</span></span>|<span data-ttu-id="40366-133">ブール</span><span class="sxs-lookup"><span data-stu-id="40366-133">boolean</span></span>|<span data-ttu-id="40366-134">内部エラーのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="40366-134">Internal used only.</span></span>|
|<span data-ttu-id="40366-135">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="40366-135">maxElavationDuration</span></span>|<span data-ttu-id="40366-136">duration</span><span class="sxs-lookup"><span data-stu-id="40366-136">duration</span></span>|<span data-ttu-id="40366-137">アクティブ化されたロールの最大の期間です。</span><span class="sxs-lookup"><span data-stu-id="40366-137">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="40366-138">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="40366-138">mfaOnElevation</span></span>|<span data-ttu-id="40366-139">ブール</span><span class="sxs-lookup"><span data-stu-id="40366-139">boolean</span></span>|<span data-ttu-id="40366-140">**true** MFA は、ロールをアクティブにするために必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="40366-140">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="40366-141">**false**場合は、MFA は、ロールをアクティブにする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="40366-141">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="40366-142">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="40366-142">minElevationDuration</span></span>|<span data-ttu-id="40366-143">duration</span><span class="sxs-lookup"><span data-stu-id="40366-143">duration</span></span>|<span data-ttu-id="40366-144">アクティブ化されたロールの最低限の期間です。</span><span class="sxs-lookup"><span data-stu-id="40366-144">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="40366-145">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="40366-145">notificationToUserOnElevation</span></span>|<span data-ttu-id="40366-146">ブール</span><span class="sxs-lookup"><span data-stu-id="40366-146">boolean</span></span>|<span data-ttu-id="40366-147">**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="40366-147">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="40366-148">**false**場合は、ロールがアクティブになったときに通知を送信できません。</span><span class="sxs-lookup"><span data-stu-id="40366-148">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="40366-149">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="40366-149">ticketingInfoOnElevation</span></span>|<span data-ttu-id="40366-150">ブール</span><span class="sxs-lookup"><span data-stu-id="40366-150">boolean</span></span>|<span data-ttu-id="40366-151">**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="40366-151">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="40366-152">**false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="40366-152">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="40366-153">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="40366-153">approvalOnElevation</span></span>|<span data-ttu-id="40366-154">ブール</span><span class="sxs-lookup"><span data-stu-id="40366-154">boolean</span></span>|<span data-ttu-id="40366-155">**true の**場合は、承認が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="40366-155">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="40366-156">**false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="40366-156">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="40366-157">approverIds</span><span class="sxs-lookup"><span data-stu-id="40366-157">approverIds</span></span>|<span data-ttu-id="40366-158">配列</span><span class="sxs-lookup"><span data-stu-id="40366-158">array</span></span>|<span data-ttu-id="40366-159">承認 id、ライセンス認証の必要な場合は承認の一覧です。</span><span class="sxs-lookup"><span data-stu-id="40366-159">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40366-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="40366-160">Relationships</span></span>
<span data-ttu-id="40366-161">なし</span><span class="sxs-lookup"><span data-stu-id="40366-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="40366-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40366-162">JSON representation</span></span>

<span data-ttu-id="40366-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40366-163">Here is a JSON representation of the resource.</span></span>

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