---
title: governanceRoleDefinition リソースの種類
description: ロール定義を表します。 azure リソースの場合は、所有者、リーダー、共同作成者など、azure RBAC の役割を表すことができます。
localization_priority: Normal
ms.openlocfilehash: 27b4b144f834f3b5eb4270a2875da5add10efb9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333758"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="64b10-104">governanceRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64b10-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="64b10-105">ロール定義を表します。</span><span class="sxs-lookup"><span data-stu-id="64b10-105">Represents the role definitions.</span></span> <span data-ttu-id="64b10-106">azure リソースの場合は、所有者、リーダー、共同作成者など、azure RBAC の役割を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="64b10-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="64b10-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="64b10-107">Methods</span></span>

| <span data-ttu-id="64b10-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="64b10-108">Method</span></span>          | <span data-ttu-id="64b10-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="64b10-109">Return Type</span></span> |<span data-ttu-id="64b10-110">説明</span><span class="sxs-lookup"><span data-stu-id="64b10-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="64b10-111">List</span><span class="sxs-lookup"><span data-stu-id="64b10-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="64b10-112">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="64b10-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="64b10-113">リソースのロール定義のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="64b10-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="64b10-114">Get</span><span class="sxs-lookup"><span data-stu-id="64b10-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="64b10-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="64b10-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="64b10-116">id で指定されたロール定義エンティティのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="64b10-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="64b10-117">`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`</span><span class="sxs-lookup"><span data-stu-id="64b10-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="64b10-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64b10-118">Properties</span></span>
| <span data-ttu-id="64b10-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64b10-119">Property</span></span>  | <span data-ttu-id="64b10-120">型</span><span class="sxs-lookup"><span data-stu-id="64b10-120">Type</span></span>      |<span data-ttu-id="64b10-121">説明</span><span class="sxs-lookup"><span data-stu-id="64b10-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="64b10-122">id</span><span class="sxs-lookup"><span data-stu-id="64b10-122">id</span></span>         |<span data-ttu-id="64b10-123">String</span><span class="sxs-lookup"><span data-stu-id="64b10-123">String</span></span>     |<span data-ttu-id="64b10-124">ロール定義の id。</span><span class="sxs-lookup"><span data-stu-id="64b10-124">The id of the role definition.</span></span> |
|<span data-ttu-id="64b10-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="64b10-125">resourceId</span></span> |<span data-ttu-id="64b10-126">String</span><span class="sxs-lookup"><span data-stu-id="64b10-126">String</span></span>     |<span data-ttu-id="64b10-127">必須。</span><span class="sxs-lookup"><span data-stu-id="64b10-127">Required.</span></span> <span data-ttu-id="64b10-128">ロール定義に関連付けられているリソースの id。</span><span class="sxs-lookup"><span data-stu-id="64b10-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="64b10-129">externalId</span><span class="sxs-lookup"><span data-stu-id="64b10-129">externalId</span></span>   |<span data-ttu-id="64b10-130">String</span><span class="sxs-lookup"><span data-stu-id="64b10-130">String</span></span>     |<span data-ttu-id="64b10-131">ロール定義の外部 id。</span><span class="sxs-lookup"><span data-stu-id="64b10-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="64b10-132">displayName</span><span class="sxs-lookup"><span data-stu-id="64b10-132">displayName</span></span>|<span data-ttu-id="64b10-133">文字列</span><span class="sxs-lookup"><span data-stu-id="64b10-133">String</span></span>     |<span data-ttu-id="64b10-134">ロール定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="64b10-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="64b10-135">templateId</span><span class="sxs-lookup"><span data-stu-id="64b10-135">templateId</span></span> | <span data-ttu-id="64b10-136">String</span><span class="sxs-lookup"><span data-stu-id="64b10-136">String</span></span> | |

## <a name="relationships"></a><span data-ttu-id="64b10-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64b10-137">Relationships</span></span>
| <span data-ttu-id="64b10-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64b10-138">Relationship</span></span> | <span data-ttu-id="64b10-139">型</span><span class="sxs-lookup"><span data-stu-id="64b10-139">Type</span></span>   |<span data-ttu-id="64b10-140">説明</span><span class="sxs-lookup"><span data-stu-id="64b10-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64b10-141">リソース</span><span class="sxs-lookup"><span data-stu-id="64b10-141">resource</span></span>|[<span data-ttu-id="64b10-142">governanceResource</span><span class="sxs-lookup"><span data-stu-id="64b10-142">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="64b10-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="64b10-143">Read-only.</span></span> <span data-ttu-id="64b10-144">ロール定義に関連付けられているリソース。</span><span class="sxs-lookup"><span data-stu-id="64b10-144">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="64b10-145">rolesetting</span><span class="sxs-lookup"><span data-stu-id="64b10-145">roleSetting</span></span>|[<span data-ttu-id="64b10-146">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="64b10-146">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="64b10-147">ロール定義に関連付けられているロール設定。</span><span class="sxs-lookup"><span data-stu-id="64b10-147">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64b10-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64b10-148">JSON representation</span></span>

<span data-ttu-id="64b10-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64b10-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",  
  "templateId":"String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
