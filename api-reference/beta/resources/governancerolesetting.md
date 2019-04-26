---
title: governanceRoleSetting リソースの種類
description: " ルールなど。"
localization_priority: Normal
ms.openlocfilehash: 09e8cb65f8318294d483a2ad66a7119d7b48822a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340227"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="b50e4-103">governanceRoleSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b50e4-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b50e4-104">役割の割り当てが作成または変更されたときに評価する必要がある各ロール定義の構成のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="b50e4-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="b50e4-105">たとえば、役割の設定には "最大割り当て期間" ルール、"アクティブ化に必要な MFA" ルールなどが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b50e4-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="b50e4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b50e4-106">Methods</span></span>

| <span data-ttu-id="b50e4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b50e4-107">Method</span></span>          | <span data-ttu-id="b50e4-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b50e4-108">Return Type</span></span> |<span data-ttu-id="b50e4-109">説明</span><span class="sxs-lookup"><span data-stu-id="b50e4-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="b50e4-110">List</span><span class="sxs-lookup"><span data-stu-id="b50e4-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="b50e4-111">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b50e4-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="b50e4-112">リソースのロール設定のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b50e4-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="b50e4-113">Get</span><span class="sxs-lookup"><span data-stu-id="b50e4-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="b50e4-114">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="b50e4-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="b50e4-115">役割設定のプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b50e4-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="b50e4-116">更新する</span><span class="sxs-lookup"><span data-stu-id="b50e4-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="b50e4-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="b50e4-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="b50e4-118">役割設定オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b50e4-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b50e4-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b50e4-119">Properties</span></span>
|<span data-ttu-id="b50e4-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b50e4-120">Property</span></span>               |<span data-ttu-id="b50e4-121">型</span><span class="sxs-lookup"><span data-stu-id="b50e4-121">Type</span></span>                                      |<span data-ttu-id="b50e4-122">説明</span><span class="sxs-lookup"><span data-stu-id="b50e4-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="b50e4-123">id</span><span class="sxs-lookup"><span data-stu-id="b50e4-123">id</span></span>                   |<span data-ttu-id="b50e4-124">String</span><span class="sxs-lookup"><span data-stu-id="b50e4-124">String</span></span>                                  |<span data-ttu-id="b50e4-125">rolesetting の id。</span><span class="sxs-lookup"><span data-stu-id="b50e4-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="b50e4-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="b50e4-126">resourceId</span></span>           |<span data-ttu-id="b50e4-127">String</span><span class="sxs-lookup"><span data-stu-id="b50e4-127">String</span></span>                                  |<span data-ttu-id="b50e4-128">必須。</span><span class="sxs-lookup"><span data-stu-id="b50e4-128">Required.</span></span> <span data-ttu-id="b50e4-129">ロール設定が関連付けられているリソースの id。</span><span class="sxs-lookup"><span data-stu-id="b50e4-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="b50e4-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b50e4-130">roleDefinitionId</span></span>     |<span data-ttu-id="b50e4-131">String</span><span class="sxs-lookup"><span data-stu-id="b50e4-131">String</span></span>                                  |<span data-ttu-id="b50e4-132">必須。</span><span class="sxs-lookup"><span data-stu-id="b50e4-132">Required.</span></span> <span data-ttu-id="b50e4-133">ロール設定が関連付けられているロール定義の id。</span><span class="sxs-lookup"><span data-stu-id="b50e4-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="b50e4-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="b50e4-134">isDefault</span></span>            |<span data-ttu-id="b50e4-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="b50e4-135">Boolean</span></span>                                 |<span data-ttu-id="b50e4-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b50e4-136">Read-only.</span></span> <span data-ttu-id="b50e4-137">rolesetting が既定の rolesetting であるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="b50e4-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="b50e4-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b50e4-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="b50e4-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b50e4-139">DateTimeOffset</span></span>                          |<span data-ttu-id="b50e4-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b50e4-140">Read-only.</span></span> <span data-ttu-id="b50e4-141">役割の設定が最後に更新された時刻。</span><span class="sxs-lookup"><span data-stu-id="b50e4-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="b50e4-142">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="b50e4-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b50e4-143">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b50e4-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b50e4-144">lastupdatedby</span><span class="sxs-lookup"><span data-stu-id="b50e4-144">lastUpdatedBy</span></span>        |<span data-ttu-id="b50e4-145">String</span><span class="sxs-lookup"><span data-stu-id="b50e4-145">String</span></span>                                  |<span data-ttu-id="b50e4-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b50e4-146">Read-only.</span></span> <span data-ttu-id="b50e4-147">rolesetting を最後に更新した管理者の表示名。</span><span class="sxs-lookup"><span data-stu-id="b50e4-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="b50e4-148">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="b50e4-148">adminEligibleSettings</span></span>|<span data-ttu-id="b50e4-149">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b50e4-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b50e4-150">管理者が対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="b50e4-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="b50e4-151">adminmembersettings</span><span class="sxs-lookup"><span data-stu-id="b50e4-151">adminMemberSettings</span></span>  |<span data-ttu-id="b50e4-152">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b50e4-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b50e4-153">管理者が直接メンバーの役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="b50e4-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="b50e4-154">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="b50e4-154">userEligibleSettings</span></span> |<span data-ttu-id="b50e4-155">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b50e4-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b50e4-156">ユーザーが対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="b50e4-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="b50e4-157">現時点では、この設定はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b50e4-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="b50e4-158">usermembersettings</span><span class="sxs-lookup"><span data-stu-id="b50e4-158">userMemberSettings</span></span>   |<span data-ttu-id="b50e4-159">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b50e4-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b50e4-160">ユーザーが役割の割り当てをアクティブ化しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="b50e4-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b50e4-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b50e4-161">Relationships</span></span>
| <span data-ttu-id="b50e4-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b50e4-162">Relationship</span></span> | <span data-ttu-id="b50e4-163">型</span><span class="sxs-lookup"><span data-stu-id="b50e4-163">Type</span></span>   |<span data-ttu-id="b50e4-164">説明</span><span class="sxs-lookup"><span data-stu-id="b50e4-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b50e4-165">リソース</span><span class="sxs-lookup"><span data-stu-id="b50e4-165">resource</span></span>|[<span data-ttu-id="b50e4-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="b50e4-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="b50e4-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b50e4-167">Read-only.</span></span> <span data-ttu-id="b50e4-168">このロール設定に関連付けられたリソース。</span><span class="sxs-lookup"><span data-stu-id="b50e4-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="b50e4-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b50e4-169">roleDefinition</span></span>|[<span data-ttu-id="b50e4-170">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b50e4-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="b50e4-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b50e4-171">Read-only.</span></span> <span data-ttu-id="b50e4-172">このロール設定で適用されるロール定義。</span><span class="sxs-lookup"><span data-stu-id="b50e4-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b50e4-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b50e4-173">JSON representation</span></span>

<span data-ttu-id="b50e4-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b50e4-174">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
