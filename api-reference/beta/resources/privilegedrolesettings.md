---
title: privilegedRoleSettings リソースの種類
description: 特権を持つロールの設定を表します。
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525697"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="5826e-103">privilegedRoleSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5826e-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5826e-104">特権を持つロールの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="5826e-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="5826e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5826e-105">Methods</span></span>

| <span data-ttu-id="5826e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5826e-106">Method</span></span>           | <span data-ttu-id="5826e-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5826e-107">Return Type</span></span>    |<span data-ttu-id="5826e-108">説明</span><span class="sxs-lookup"><span data-stu-id="5826e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5826e-109">PrivilegedRoleSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="5826e-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="5826e-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5826e-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="5826e-111">PrivilegedRoleSettings オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5826e-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="5826e-112">PrivilegedRoleSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="5826e-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="5826e-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5826e-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="5826e-114">PrivilegedRoleSettings オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5826e-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="5826e-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5826e-115">Properties</span></span>
| <span data-ttu-id="5826e-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5826e-116">Property</span></span>     | <span data-ttu-id="5826e-117">型</span><span class="sxs-lookup"><span data-stu-id="5826e-117">Type</span></span>   |<span data-ttu-id="5826e-118">説明</span><span class="sxs-lookup"><span data-stu-id="5826e-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5826e-119">ElevationDuration</span><span class="sxs-lookup"><span data-stu-id="5826e-119">elevationDuration</span></span>|<span data-ttu-id="5826e-120">duration</span><span class="sxs-lookup"><span data-stu-id="5826e-120">duration</span></span>|<span data-ttu-id="5826e-121">ロールが有効な場合の期間です。</span><span class="sxs-lookup"><span data-stu-id="5826e-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="5826e-122">id</span><span class="sxs-lookup"><span data-stu-id="5826e-122">id</span></span>|<span data-ttu-id="5826e-123">string</span><span class="sxs-lookup"><span data-stu-id="5826e-123">string</span></span>| <span data-ttu-id="5826e-124">ロールの設定の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5826e-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="5826e-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5826e-125">Read-only.</span></span>|
|<span data-ttu-id="5826e-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="5826e-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="5826e-127">boolean</span><span class="sxs-lookup"><span data-stu-id="5826e-127">boolean</span></span>|<span data-ttu-id="5826e-128">**真**mfaOnElevation は、構成可能な場合です。</span><span class="sxs-lookup"><span data-stu-id="5826e-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="5826e-129">場合は**false を指定**mfaOnElevation は構成できません。</span><span class="sxs-lookup"><span data-stu-id="5826e-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="5826e-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="5826e-130">lastGlobalAdmin</span></span>|<span data-ttu-id="5826e-131">boolean</span><span class="sxs-lookup"><span data-stu-id="5826e-131">boolean</span></span>|<span data-ttu-id="5826e-132">内部エラーのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="5826e-132">Internal used only.</span></span>|
|<span data-ttu-id="5826e-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="5826e-133">maxElavationDuration</span></span>|<span data-ttu-id="5826e-134">duration</span><span class="sxs-lookup"><span data-stu-id="5826e-134">duration</span></span>|<span data-ttu-id="5826e-135">アクティブ化されたロールの最大の期間です。</span><span class="sxs-lookup"><span data-stu-id="5826e-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="5826e-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="5826e-136">mfaOnElevation</span></span>|<span data-ttu-id="5826e-137">boolean</span><span class="sxs-lookup"><span data-stu-id="5826e-137">boolean</span></span>|<span data-ttu-id="5826e-138">**true** MFA は、ロールをアクティブにするために必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="5826e-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="5826e-139">**false**場合は、MFA は、ロールをアクティブにする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="5826e-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="5826e-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="5826e-140">minElevationDuration</span></span>|<span data-ttu-id="5826e-141">duration</span><span class="sxs-lookup"><span data-stu-id="5826e-141">duration</span></span>|<span data-ttu-id="5826e-142">アクティブ化されたロールの最低限の期間です。</span><span class="sxs-lookup"><span data-stu-id="5826e-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="5826e-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="5826e-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="5826e-144">boolean</span><span class="sxs-lookup"><span data-stu-id="5826e-144">boolean</span></span>|<span data-ttu-id="5826e-145">**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="5826e-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="5826e-146">**false**場合は、ロールがアクティブになったときに通知を送信できません。</span><span class="sxs-lookup"><span data-stu-id="5826e-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="5826e-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="5826e-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="5826e-148">boolean</span><span class="sxs-lookup"><span data-stu-id="5826e-148">boolean</span></span>|<span data-ttu-id="5826e-149">**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="5826e-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="5826e-150">**false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="5826e-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="5826e-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="5826e-151">approvalOnElevation</span></span>|<span data-ttu-id="5826e-152">boolean</span><span class="sxs-lookup"><span data-stu-id="5826e-152">boolean</span></span>|<span data-ttu-id="5826e-153">**true の**場合は、承認が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="5826e-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="5826e-154">**false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="5826e-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="5826e-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="5826e-155">approverIds</span></span>|<span data-ttu-id="5826e-156">配列</span><span class="sxs-lookup"><span data-stu-id="5826e-156">array</span></span>|<span data-ttu-id="5826e-157">承認 id、ライセンス認証の必要な場合は承認の一覧です。</span><span class="sxs-lookup"><span data-stu-id="5826e-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5826e-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5826e-158">Relationships</span></span>
<span data-ttu-id="5826e-159">なし</span><span class="sxs-lookup"><span data-stu-id="5826e-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5826e-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5826e-160">JSON representation</span></span>

<span data-ttu-id="5826e-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5826e-161">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
