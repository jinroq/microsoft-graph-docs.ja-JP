---
title: groupLifecyclePolicy リソース タイプ
description: Office 365 グループのライフサイクルポリシーを表します。 グループのライフサイクル ポリシーにより、管理者はグループに対して有効期限を設定できます。 たとえば、180 日後にグループの有効期限が切れます。 グループの有効期限に達すると、グループの所有者は、管理者が定義した時間間隔内でグループを更新する必要があります。 更新されると、グループの有効期限はポリシーで定義された日数、延長されます。 たとえば、グループの新しい有効期限は、更新後 180 日です。 グループが更新されない場合、グループの有効期限が切れ、削除されます。 グループは、削除から 30 日以内に復元できます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7eccede97fb4f9eafc69a04136612c30ad2c27ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971831"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="22626-110">groupLifecyclePolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="22626-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="22626-111">Office 365 グループのライフサイクルポリシーを表します。</span><span class="sxs-lookup"><span data-stu-id="22626-111">Represents a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="22626-112">グループのライフサイクル ポリシーにより、管理者はグループに対して有効期限を設定できます。</span><span class="sxs-lookup"><span data-stu-id="22626-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="22626-113">たとえば、180 日後にグループの有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="22626-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="22626-114">グループの有効期限に達すると、グループの所有者は、管理者が定義した時間間隔内でグループを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="22626-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="22626-115">更新されると、グループの有効期限はポリシーで定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="22626-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="22626-116">たとえば、グループの新しい有効期限は、更新後 180 日です。</span><span class="sxs-lookup"><span data-stu-id="22626-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="22626-117">グループが更新されない場合、グループの有効期限が切れ、削除されます。</span><span class="sxs-lookup"><span data-stu-id="22626-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="22626-118">グループは、削除から 30 日以内に復元できます。</span><span class="sxs-lookup"><span data-stu-id="22626-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="22626-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="22626-119">Methods</span></span>

| <span data-ttu-id="22626-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="22626-120">Method</span></span> | <span data-ttu-id="22626-121">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="22626-121">Return Type</span></span> | <span data-ttu-id="22626-122">説明</span><span class="sxs-lookup"><span data-stu-id="22626-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="22626-123">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="22626-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="22626-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="22626-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="22626-125">groupLifecyclePolicy オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="22626-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="22626-126">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="22626-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="22626-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22626-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="22626-128">すべての groupLifecyclePolicies を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="22626-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="22626-129">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="22626-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="22626-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="22626-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="22626-131">groupLifecyclePolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="22626-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="22626-132">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="22626-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="22626-133">None</span><span class="sxs-lookup"><span data-stu-id="22626-133">None</span></span> | <span data-ttu-id="22626-134">groupLifecyclePolicy オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="22626-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="22626-135">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="22626-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="22626-136">None</span><span class="sxs-lookup"><span data-stu-id="22626-136">None</span></span>| <span data-ttu-id="22626-137">ライフ サイクル ポリシーにグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="22626-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="22626-138">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="22626-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="22626-139">なし</span><span class="sxs-lookup"><span data-stu-id="22626-139">None</span></span>| <span data-ttu-id="22626-140">ライフ サイクル ポリシーからグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="22626-140">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="22626-141">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="22626-141">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="22626-142">None</span><span class="sxs-lookup"><span data-stu-id="22626-142">None</span></span>| <span data-ttu-id="22626-143">グループの有効期限を更新します。</span><span class="sxs-lookup"><span data-stu-id="22626-143">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="22626-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22626-144">Properties</span></span>

| <span data-ttu-id="22626-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22626-145">Property</span></span> | <span data-ttu-id="22626-146">型</span><span class="sxs-lookup"><span data-stu-id="22626-146">Type</span></span> | <span data-ttu-id="22626-147">説明</span><span class="sxs-lookup"><span data-stu-id="22626-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="22626-148">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="22626-148">alternateNotificationEmails</span></span>|<span data-ttu-id="22626-149">String</span><span class="sxs-lookup"><span data-stu-id="22626-149">String</span></span>| <span data-ttu-id="22626-150">所有者のいないグループに対して通知を送信する電子メール アドレスのリスト</span><span class="sxs-lookup"><span data-stu-id="22626-150">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="22626-151">電子メール アドレスをセミコロンで区切って、複数の電子メール アドレスを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="22626-151">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="22626-152">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="22626-152">groupLifetimeInDays</span></span>|<span data-ttu-id="22626-153">Int32</span><span class="sxs-lookup"><span data-stu-id="22626-153">Int32</span></span>| <span data-ttu-id="22626-154">グループの有効期限が切れ、更新が必要になるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="22626-154">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="22626-155">更新されると、グループの有効期限は定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="22626-155">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="22626-156">id</span><span class="sxs-lookup"><span data-stu-id="22626-156">id</span></span>|<span data-ttu-id="22626-157">Guid</span><span class="sxs-lookup"><span data-stu-id="22626-157">Guid</span></span>| <span data-ttu-id="22626-158">ポリシーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="22626-158">A unique identifier for a policy.</span></span> <span data-ttu-id="22626-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="22626-159">Read-only.</span></span>|
|<span data-ttu-id="22626-160">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="22626-160">managedGroupTypes</span></span>|<span data-ttu-id="22626-161">String</span><span class="sxs-lookup"><span data-stu-id="22626-161">String</span></span>| <span data-ttu-id="22626-162">有効期限ポリシーを適用するグループの種類。</span><span class="sxs-lookup"><span data-stu-id="22626-162">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="22626-163">可能な値は、**All**、**Selected**、または **None** です。</span><span class="sxs-lookup"><span data-stu-id="22626-163">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="22626-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22626-164">Relationships</span></span>

<span data-ttu-id="22626-165">なし。</span><span class="sxs-lookup"><span data-stu-id="22626-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="22626-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22626-166">JSON representation</span></span>

<span data-ttu-id="22626-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22626-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
