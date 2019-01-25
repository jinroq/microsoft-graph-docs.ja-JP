---
title: governanceRoleSetting リソースの種類
description: " ルールというように。"
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508168"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="9800c-103">governanceRoleSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9800c-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9800c-104">各役割の割り当ての作成または変更されたときに、に対して評価する必要がある役割の定義の構成のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="9800c-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="9800c-105">たとえば、ロールの設定は、[最大割り当て期間] のルール、ルールの「ライセンス認証に必要な MFA」などがあります。</span><span class="sxs-lookup"><span data-stu-id="9800c-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="9800c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="9800c-106">Methods</span></span>

| <span data-ttu-id="9800c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9800c-107">Method</span></span>          | <span data-ttu-id="9800c-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9800c-108">Return Type</span></span> |<span data-ttu-id="9800c-109">説明</span><span class="sxs-lookup"><span data-stu-id="9800c-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="9800c-110">List</span><span class="sxs-lookup"><span data-stu-id="9800c-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="9800c-111">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9800c-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="9800c-112">リソースのロールの設定の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="9800c-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="9800c-113">Get</span><span class="sxs-lookup"><span data-stu-id="9800c-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="9800c-114">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="9800c-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="9800c-115">ロール設定のプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9800c-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="9800c-116">Update</span><span class="sxs-lookup"><span data-stu-id="9800c-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="9800c-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="9800c-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="9800c-118">ロールの設定オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9800c-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9800c-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9800c-119">Properties</span></span>
|<span data-ttu-id="9800c-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9800c-120">Property</span></span>               |<span data-ttu-id="9800c-121">型</span><span class="sxs-lookup"><span data-stu-id="9800c-121">Type</span></span>                                      |<span data-ttu-id="9800c-122">説明</span><span class="sxs-lookup"><span data-stu-id="9800c-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="9800c-123">id</span><span class="sxs-lookup"><span data-stu-id="9800c-123">id</span></span>                   |<span data-ttu-id="9800c-124">String</span><span class="sxs-lookup"><span data-stu-id="9800c-124">String</span></span>                                  |<span data-ttu-id="9800c-125">RoleSetting の id です。</span><span class="sxs-lookup"><span data-stu-id="9800c-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="9800c-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="9800c-126">resourceId</span></span>           |<span data-ttu-id="9800c-127">String</span><span class="sxs-lookup"><span data-stu-id="9800c-127">String</span></span>                                  |<span data-ttu-id="9800c-128">必須。</span><span class="sxs-lookup"><span data-stu-id="9800c-128">Required.</span></span> <span data-ttu-id="9800c-129">役割の設定が関連付けられているリソースの id です。</span><span class="sxs-lookup"><span data-stu-id="9800c-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="9800c-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9800c-130">roleDefinitionId</span></span>     |<span data-ttu-id="9800c-131">String</span><span class="sxs-lookup"><span data-stu-id="9800c-131">String</span></span>                                  |<span data-ttu-id="9800c-132">必須。</span><span class="sxs-lookup"><span data-stu-id="9800c-132">Required.</span></span> <span data-ttu-id="9800c-133">役割の設定が関連付けられている役割の定義の id です。</span><span class="sxs-lookup"><span data-stu-id="9800c-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="9800c-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="9800c-134">isDefault</span></span>            |<span data-ttu-id="9800c-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="9800c-135">Boolean</span></span>                                 |<span data-ttu-id="9800c-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9800c-136">Read-only.</span></span> <span data-ttu-id="9800c-137">RoleSetting がデフォルトの roleSetting であることを示す</span><span class="sxs-lookup"><span data-stu-id="9800c-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="9800c-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9800c-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="9800c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9800c-139">DateTimeOffset</span></span>                          |<span data-ttu-id="9800c-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9800c-140">Read-only.</span></span> <span data-ttu-id="9800c-141">役割の設定が最後に更新された時刻。</span><span class="sxs-lookup"><span data-stu-id="9800c-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="9800c-142">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="9800c-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9800c-143">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9800c-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9800c-144">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="9800c-144">lastUpdatedBy</span></span>        |<span data-ttu-id="9800c-145">String</span><span class="sxs-lookup"><span data-stu-id="9800c-145">String</span></span>                                  |<span data-ttu-id="9800c-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9800c-146">Read-only.</span></span> <span data-ttu-id="9800c-147">RoleSetting を最後に更新した管理者の表示名。</span><span class="sxs-lookup"><span data-stu-id="9800c-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="9800c-148">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="9800c-148">adminEligibleSettings</span></span>|<span data-ttu-id="9800c-149">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9800c-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="9800c-150">管理者対象のロール割り当てを追加しようとするときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="9800c-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="9800c-151">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="9800c-151">adminMemberSettings</span></span>  |<span data-ttu-id="9800c-152">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9800c-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="9800c-153">直接的なメンバーの役割の割り当てを追加する際に管理者に評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="9800c-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="9800c-154">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="9800c-154">userEligibleSettings</span></span> |<span data-ttu-id="9800c-155">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9800c-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="9800c-156">ユーザーが対象のロール割り当てを追加するときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="9800c-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="9800c-157">設定は、ここではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9800c-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="9800c-158">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="9800c-158">userMemberSettings</span></span>   |<span data-ttu-id="9800c-159">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9800c-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="9800c-160">ユーザーが彼の役割の割り当てを有効にしようとした場合に評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="9800c-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9800c-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9800c-161">Relationships</span></span>
| <span data-ttu-id="9800c-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9800c-162">Relationship</span></span> | <span data-ttu-id="9800c-163">型</span><span class="sxs-lookup"><span data-stu-id="9800c-163">Type</span></span>   |<span data-ttu-id="9800c-164">説明</span><span class="sxs-lookup"><span data-stu-id="9800c-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9800c-165">リソース</span><span class="sxs-lookup"><span data-stu-id="9800c-165">resource</span></span>|[<span data-ttu-id="9800c-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="9800c-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="9800c-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9800c-167">Read-only.</span></span> <span data-ttu-id="9800c-168">このロールの設定に関連付けられているリソースです。</span><span class="sxs-lookup"><span data-stu-id="9800c-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="9800c-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9800c-169">roleDefinition</span></span>|[<span data-ttu-id="9800c-170">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9800c-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="9800c-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9800c-171">Read-only.</span></span> <span data-ttu-id="9800c-172">役割の定義を適用するこのロールの設定をします。</span><span class="sxs-lookup"><span data-stu-id="9800c-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9800c-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9800c-173">JSON representation</span></span>

<span data-ttu-id="9800c-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9800c-174">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
