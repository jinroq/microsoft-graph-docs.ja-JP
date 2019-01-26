---
title: privilegedRoleSettings リソースの種類
description: 特権を持つロールの設定を表します。
localization_priority: Normal
ms.openlocfilehash: 673327e3c83a4111eb469ca48550836433dbdf0a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577152"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="c1680-103">privilegedRoleSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1680-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1680-104">特権を持つロールの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="c1680-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="c1680-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1680-105">Methods</span></span>

| <span data-ttu-id="c1680-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1680-106">Method</span></span>           | <span data-ttu-id="c1680-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c1680-107">Return Type</span></span>    |<span data-ttu-id="c1680-108">説明</span><span class="sxs-lookup"><span data-stu-id="c1680-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1680-109">PrivilegedRoleSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="c1680-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="c1680-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c1680-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="c1680-111">PrivilegedRoleSettings オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1680-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="c1680-112">PrivilegedRoleSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="c1680-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="c1680-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c1680-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="c1680-114">PrivilegedRoleSettings オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c1680-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="c1680-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1680-115">Properties</span></span>
| <span data-ttu-id="c1680-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1680-116">Property</span></span>     | <span data-ttu-id="c1680-117">型</span><span class="sxs-lookup"><span data-stu-id="c1680-117">Type</span></span>   |<span data-ttu-id="c1680-118">説明</span><span class="sxs-lookup"><span data-stu-id="c1680-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1680-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="c1680-119">elevationDuration</span></span>| <span data-ttu-id="c1680-120">文字列 (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="c1680-120">String (timestamp)</span></span> |<span data-ttu-id="c1680-121">ロールが有効な場合の期間です。</span><span class="sxs-lookup"><span data-stu-id="c1680-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="c1680-122">id</span><span class="sxs-lookup"><span data-stu-id="c1680-122">id</span></span>| <span data-ttu-id="c1680-123">文字列 (識別子)</span><span class="sxs-lookup"><span data-stu-id="c1680-123">string (identifier)</span></span>| <span data-ttu-id="c1680-124">ロールの設定の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c1680-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="c1680-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c1680-125">Read-only.</span></span>|
|<span data-ttu-id="c1680-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="c1680-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="c1680-127">boolean</span><span class="sxs-lookup"><span data-stu-id="c1680-127">boolean</span></span>|<span data-ttu-id="c1680-128">**真**mfaOnElevation は、構成可能な場合です。</span><span class="sxs-lookup"><span data-stu-id="c1680-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="c1680-129">場合は**false を指定**mfaOnElevation は構成できません。</span><span class="sxs-lookup"><span data-stu-id="c1680-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="c1680-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="c1680-130">lastGlobalAdmin</span></span>|<span data-ttu-id="c1680-131">boolean</span><span class="sxs-lookup"><span data-stu-id="c1680-131">boolean</span></span>|<span data-ttu-id="c1680-132">内部エラーのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="c1680-132">Internal used only.</span></span>|
|<span data-ttu-id="c1680-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="c1680-133">maxElavationDuration</span></span>| <span data-ttu-id="c1680-134">文字列 (識別子)</span><span class="sxs-lookup"><span data-stu-id="c1680-134">string (identifier)</span></span>| |<span data-ttu-id="c1680-135">アクティブ化されたロールの最大の期間です。</span><span class="sxs-lookup"><span data-stu-id="c1680-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="c1680-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="c1680-136">mfaOnElevation</span></span>|<span data-ttu-id="c1680-137">boolean</span><span class="sxs-lookup"><span data-stu-id="c1680-137">boolean</span></span>|<span data-ttu-id="c1680-138">**true** MFA は、ロールをアクティブにするために必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="c1680-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="c1680-139">**false**場合は、MFA は、ロールをアクティブにする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="c1680-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="c1680-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="c1680-140">minElevationDuration</span></span>|<span data-ttu-id="c1680-141">文字列 (識別子)</span><span class="sxs-lookup"><span data-stu-id="c1680-141">string (identifier)</span></span>||<span data-ttu-id="c1680-142">アクティブ化されたロールの最低限の期間です。</span><span class="sxs-lookup"><span data-stu-id="c1680-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="c1680-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="c1680-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="c1680-144">boolean</span><span class="sxs-lookup"><span data-stu-id="c1680-144">boolean</span></span>|<span data-ttu-id="c1680-145">**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="c1680-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="c1680-146">**false**場合は、ロールがアクティブになったときに通知を送信できません。</span><span class="sxs-lookup"><span data-stu-id="c1680-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="c1680-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="c1680-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="c1680-148">boolean</span><span class="sxs-lookup"><span data-stu-id="c1680-148">boolean</span></span>|<span data-ttu-id="c1680-149">**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="c1680-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="c1680-150">**false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="c1680-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="c1680-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="c1680-151">approvalOnElevation</span></span>|<span data-ttu-id="c1680-152">boolean</span><span class="sxs-lookup"><span data-stu-id="c1680-152">boolean</span></span>|<span data-ttu-id="c1680-153">**true の**場合は、承認が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="c1680-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="c1680-154">**false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="c1680-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="c1680-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="c1680-155">approverIds</span></span>| <span data-ttu-id="c1680-156">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1680-156">String collection</span></span> |<span data-ttu-id="c1680-157">承認 id、ライセンス認証の必要な場合は承認の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c1680-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1680-158">関係</span><span class="sxs-lookup"><span data-stu-id="c1680-158">Relationships</span></span>
<span data-ttu-id="c1680-159">なし</span><span class="sxs-lookup"><span data-stu-id="c1680-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c1680-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1680-160">JSON representation</span></span>

<span data-ttu-id="c1680-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1680-161">Here is a JSON representation of the resource.</span></span>

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
  "approverIds": [ "String (identifier)" ]
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
