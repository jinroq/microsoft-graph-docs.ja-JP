---
title: privilegedRoleSettings リソースの種類
description: 特権ロールの設定を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ed87787ca8016f1dde7711304a1da1fc977c641b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965714"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="1cc5a-103">privilegedRoleSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1cc5a-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc5a-104">特権ロールの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="1cc5a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1cc5a-105">Methods</span></span>

| <span data-ttu-id="1cc5a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1cc5a-106">Method</span></span>           | <span data-ttu-id="1cc5a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1cc5a-107">Return Type</span></span>    |<span data-ttu-id="1cc5a-108">説明</span><span class="sxs-lookup"><span data-stu-id="1cc5a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cc5a-109">privilegedRoleSettings を取得する</span><span class="sxs-lookup"><span data-stu-id="1cc5a-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="1cc5a-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="1cc5a-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="1cc5a-111">PrivilegedRoleSettings オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="1cc5a-112">PrivilegedRoleSettings の更新</span><span class="sxs-lookup"><span data-stu-id="1cc5a-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="1cc5a-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="1cc5a-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="1cc5a-114">PrivilegedRoleSettings オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="1cc5a-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cc5a-115">Properties</span></span>
| <span data-ttu-id="1cc5a-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cc5a-116">Property</span></span>     | <span data-ttu-id="1cc5a-117">型</span><span class="sxs-lookup"><span data-stu-id="1cc5a-117">Type</span></span>   |<span data-ttu-id="1cc5a-118">説明</span><span class="sxs-lookup"><span data-stu-id="1cc5a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cc5a-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="1cc5a-119">elevationDuration</span></span>|<span data-ttu-id="1cc5a-120">duration</span><span class="sxs-lookup"><span data-stu-id="1cc5a-120">duration</span></span>|<span data-ttu-id="1cc5a-121">役割がアクティブ化される期間。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="1cc5a-122">id</span><span class="sxs-lookup"><span data-stu-id="1cc5a-122">id</span></span>|<span data-ttu-id="1cc5a-123">string</span><span class="sxs-lookup"><span data-stu-id="1cc5a-123">string</span></span>| <span data-ttu-id="1cc5a-124">ロール設定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="1cc5a-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-125">Read-only.</span></span>|
|<span data-ttu-id="1cc5a-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="1cc5a-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="1cc5a-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="1cc5a-127">boolean</span></span>|<span data-ttu-id="1cc5a-128">**true**の場合は、mfaOnElevation を構成できます。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="1cc5a-129">mfaOnElevation を構成できない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="1cc5a-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="1cc5a-130">lastGlobalAdmin</span></span>|<span data-ttu-id="1cc5a-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="1cc5a-131">boolean</span></span>|<span data-ttu-id="1cc5a-132">内部でのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-132">Internal used only.</span></span>|
|<span data-ttu-id="1cc5a-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="1cc5a-133">maxElavationDuration</span></span>|<span data-ttu-id="1cc5a-134">duration</span><span class="sxs-lookup"><span data-stu-id="1cc5a-134">duration</span></span>|<span data-ttu-id="1cc5a-135">アクティブ化されたロールの最大期間。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="1cc5a-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="1cc5a-136">mfaOnElevation</span></span>|<span data-ttu-id="1cc5a-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="1cc5a-137">boolean</span></span>|<span data-ttu-id="1cc5a-138">役割をアクティブ化するために MFA が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="1cc5a-139">役割をアクティブ化するために MFA が必要でない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="1cc5a-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="1cc5a-140">minElevationDuration</span></span>|<span data-ttu-id="1cc5a-141">duration</span><span class="sxs-lookup"><span data-stu-id="1cc5a-141">duration</span></span>|<span data-ttu-id="1cc5a-142">アクティブ化されたロールの期間を最小化します。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="1cc5a-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="1cc5a-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="1cc5a-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="1cc5a-144">boolean</span></span>|<span data-ttu-id="1cc5a-145">**true**の場合は、エンドユーザーに役割がアクティブ化されたときに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="1cc5a-146">**true**の場合は、役割がアクティブ化されたときに通知を送信しません。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="1cc5a-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="1cc5a-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="1cc5a-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="1cc5a-148">boolean</span></span>|<span data-ttu-id="1cc5a-149">役割をアクティブ化するときに、チケット情報が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="1cc5a-150">**false**を指定すると、役割をアクティブ化するときに、チケットの情報は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="1cc5a-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="1cc5a-151">approvalOnElevation</span></span>|<span data-ttu-id="1cc5a-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="1cc5a-152">boolean</span></span>|<span data-ttu-id="1cc5a-153">ロールをアクティブ化するときに承認が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="1cc5a-154">**false**を指定すると、役割をアクティブ化するときに承認が必要ありません。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="1cc5a-155">承認の検証 Ds</span><span class="sxs-lookup"><span data-stu-id="1cc5a-155">approverIds</span></span>| <span data-ttu-id="1cc5a-156">string collection</span><span class="sxs-lookup"><span data-stu-id="1cc5a-156">string collection</span></span> |<span data-ttu-id="1cc5a-157">ライセンス認証に承認が必要な場合は、承認 id のリスト。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cc5a-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1cc5a-158">Relationships</span></span>
<span data-ttu-id="1cc5a-159">なし</span><span class="sxs-lookup"><span data-stu-id="1cc5a-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1cc5a-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1cc5a-160">JSON representation</span></span>

<span data-ttu-id="1cc5a-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1cc5a-161">Here is a JSON representation of the resource.</span></span>

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
  "approverIds": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
