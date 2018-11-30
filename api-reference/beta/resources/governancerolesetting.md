---
title: governanceRoleSetting リソースの種類
description: " ルールというように。"
ms.openlocfilehash: 64245b2d6f0aa9e0ea3ffda4a5eaebfb9fd205df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070765"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="346b8-103">governanceRoleSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="346b8-103">governanceRoleSetting resource type</span></span>

> <span data-ttu-id="346b8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="346b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="346b8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="346b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="346b8-106">各役割の割り当ての作成または変更されたときに、に対して評価する必要がある役割の定義の構成のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="346b8-106">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="346b8-107">たとえば、ロールの設定は、[最大割り当て期間] のルール、ルールの「ライセンス認証に必要な MFA」などがあります。</span><span class="sxs-lookup"><span data-stu-id="346b8-107">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="346b8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="346b8-108">Methods</span></span>

| <span data-ttu-id="346b8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="346b8-109">Method</span></span>          | <span data-ttu-id="346b8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="346b8-110">Return Type</span></span> |<span data-ttu-id="346b8-111">説明</span><span class="sxs-lookup"><span data-stu-id="346b8-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="346b8-112">List</span><span class="sxs-lookup"><span data-stu-id="346b8-112">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="346b8-113">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="346b8-113">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="346b8-114">リソースのロールの設定の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="346b8-114">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="346b8-115">Get</span><span class="sxs-lookup"><span data-stu-id="346b8-115">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="346b8-116">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="346b8-116">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="346b8-117">ロール設定のプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="346b8-117">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="346b8-118">Update</span><span class="sxs-lookup"><span data-stu-id="346b8-118">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="346b8-119">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="346b8-119">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="346b8-120">ロールの設定オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="346b8-120">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="346b8-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="346b8-121">Properties</span></span>
|<span data-ttu-id="346b8-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="346b8-122">Property</span></span>               |<span data-ttu-id="346b8-123">型</span><span class="sxs-lookup"><span data-stu-id="346b8-123">Type</span></span>                                      |<span data-ttu-id="346b8-124">説明</span><span class="sxs-lookup"><span data-stu-id="346b8-124">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="346b8-125">id</span><span class="sxs-lookup"><span data-stu-id="346b8-125">id</span></span>                   |<span data-ttu-id="346b8-126">String</span><span class="sxs-lookup"><span data-stu-id="346b8-126">String</span></span>                                  |<span data-ttu-id="346b8-127">RoleSetting の id です。</span><span class="sxs-lookup"><span data-stu-id="346b8-127">The id of the roleSetting.</span></span>|
|<span data-ttu-id="346b8-128">resourceId</span><span class="sxs-lookup"><span data-stu-id="346b8-128">resourceId</span></span>           |<span data-ttu-id="346b8-129">String</span><span class="sxs-lookup"><span data-stu-id="346b8-129">String</span></span>                                  |<span data-ttu-id="346b8-130">必須。</span><span class="sxs-lookup"><span data-stu-id="346b8-130">Required.</span></span> <span data-ttu-id="346b8-131">役割の設定が関連付けられているリソースの id です。</span><span class="sxs-lookup"><span data-stu-id="346b8-131">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="346b8-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="346b8-132">roleDefinitionId</span></span>     |<span data-ttu-id="346b8-133">String</span><span class="sxs-lookup"><span data-stu-id="346b8-133">String</span></span>                                  |<span data-ttu-id="346b8-134">必須。</span><span class="sxs-lookup"><span data-stu-id="346b8-134">Required.</span></span> <span data-ttu-id="346b8-135">役割の設定が関連付けられている役割の定義の id です。</span><span class="sxs-lookup"><span data-stu-id="346b8-135">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="346b8-136">isDefault</span><span class="sxs-lookup"><span data-stu-id="346b8-136">isDefault</span></span>            |<span data-ttu-id="346b8-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="346b8-137">Boolean</span></span>                                 |<span data-ttu-id="346b8-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="346b8-138">Read-only.</span></span> <span data-ttu-id="346b8-139">RoleSetting がデフォルトの roleSetting であることを示す</span><span class="sxs-lookup"><span data-stu-id="346b8-139">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="346b8-140">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="346b8-140">lastUpdatedDateTime</span></span>  |<span data-ttu-id="346b8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346b8-141">DateTimeOffset</span></span>                          |<span data-ttu-id="346b8-142">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="346b8-142">Read-only.</span></span> <span data-ttu-id="346b8-143">役割の設定が最後に更新された時刻。</span><span class="sxs-lookup"><span data-stu-id="346b8-143">The time when the role setting was last updated.</span></span> <span data-ttu-id="346b8-144">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="346b8-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="346b8-145">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="346b8-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="346b8-146">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="346b8-146">lastUpdatedBy</span></span>        |<span data-ttu-id="346b8-147">String</span><span class="sxs-lookup"><span data-stu-id="346b8-147">String</span></span>                                  |<span data-ttu-id="346b8-148">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="346b8-148">Read-only.</span></span> <span data-ttu-id="346b8-149">RoleSetting を最後に更新した管理者の表示名。</span><span class="sxs-lookup"><span data-stu-id="346b8-149">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="346b8-150">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="346b8-150">adminEligibleSettings</span></span>|<span data-ttu-id="346b8-151">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="346b8-151">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="346b8-152">管理者対象のロール割り当てを追加しようとするときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="346b8-152">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="346b8-153">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="346b8-153">adminMemberSettings</span></span>  |<span data-ttu-id="346b8-154">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="346b8-154">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="346b8-155">直接的なメンバーの役割の割り当てを追加する際に管理者に評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="346b8-155">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="346b8-156">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="346b8-156">userEligibleSettings</span></span> |<span data-ttu-id="346b8-157">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="346b8-157">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="346b8-158">ユーザーが対象のロール割り当てを追加するときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="346b8-158">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="346b8-159">設定は、ここではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="346b8-159">The setting is not supported for now.</span></span>|
|<span data-ttu-id="346b8-160">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="346b8-160">userMemberSettings</span></span>   |<span data-ttu-id="346b8-161">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="346b8-161">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="346b8-162">ユーザーが彼の役割の割り当てを有効にしようとした場合に評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="346b8-162">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="346b8-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="346b8-163">Relationships</span></span>
| <span data-ttu-id="346b8-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="346b8-164">Relationship</span></span> | <span data-ttu-id="346b8-165">型</span><span class="sxs-lookup"><span data-stu-id="346b8-165">Type</span></span>   |<span data-ttu-id="346b8-166">説明</span><span class="sxs-lookup"><span data-stu-id="346b8-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="346b8-167">リソース</span><span class="sxs-lookup"><span data-stu-id="346b8-167">resource</span></span>|[<span data-ttu-id="346b8-168">governanceResource</span><span class="sxs-lookup"><span data-stu-id="346b8-168">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="346b8-169">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="346b8-169">Read-only.</span></span> <span data-ttu-id="346b8-170">このロールの設定に関連付けられているリソースです。</span><span class="sxs-lookup"><span data-stu-id="346b8-170">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="346b8-171">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="346b8-171">roleDefinition</span></span>|[<span data-ttu-id="346b8-172">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="346b8-172">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="346b8-173">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="346b8-173">Read-only.</span></span> <span data-ttu-id="346b8-174">役割の定義を適用するこのロールの設定をします。</span><span class="sxs-lookup"><span data-stu-id="346b8-174">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="346b8-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="346b8-175">JSON representation</span></span>

<span data-ttu-id="346b8-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="346b8-176">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
