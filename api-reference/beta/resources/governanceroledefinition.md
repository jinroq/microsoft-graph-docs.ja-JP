---
title: governanceRoleDefinition リソースの種類
description: ロール定義を表します。 Azure リソースの場合は、所有者、リーダー、共同作成者など、Azure RBAC の役割を表すことができます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 668f5430e8f098986b7d5398f32c9c35543a7e11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971852"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="38e1f-104">governanceRoleDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38e1f-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="38e1f-105">ロール定義を表します。</span><span class="sxs-lookup"><span data-stu-id="38e1f-105">Represents the role definitions.</span></span> <span data-ttu-id="38e1f-106">Azure リソースの場合は、所有者、リーダー、共同作成者など、Azure RBAC の役割を表すことができます。</span><span class="sxs-lookup"><span data-stu-id="38e1f-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="38e1f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="38e1f-107">Methods</span></span>

| <span data-ttu-id="38e1f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="38e1f-108">Method</span></span>          | <span data-ttu-id="38e1f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="38e1f-109">Return Type</span></span> |<span data-ttu-id="38e1f-110">説明</span><span class="sxs-lookup"><span data-stu-id="38e1f-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="38e1f-111">List</span><span class="sxs-lookup"><span data-stu-id="38e1f-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="38e1f-112">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="38e1f-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="38e1f-113">リソースのロール定義のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="38e1f-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="38e1f-114">Get</span><span class="sxs-lookup"><span data-stu-id="38e1f-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="38e1f-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="38e1f-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="38e1f-116">Id で指定されたロール定義エンティティのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="38e1f-116">Read properties and relationships of a role definition entity specified by id.</span></span>|

<span data-ttu-id="38e1f-117">`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`</span><span class="sxs-lookup"><span data-stu-id="38e1f-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="38e1f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38e1f-118">Properties</span></span>
| <span data-ttu-id="38e1f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38e1f-119">Property</span></span>  | <span data-ttu-id="38e1f-120">型</span><span class="sxs-lookup"><span data-stu-id="38e1f-120">Type</span></span>      |<span data-ttu-id="38e1f-121">説明</span><span class="sxs-lookup"><span data-stu-id="38e1f-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="38e1f-122">id</span><span class="sxs-lookup"><span data-stu-id="38e1f-122">id</span></span>         |<span data-ttu-id="38e1f-123">文字列</span><span class="sxs-lookup"><span data-stu-id="38e1f-123">String</span></span>     |<span data-ttu-id="38e1f-124">ロール定義の id。</span><span class="sxs-lookup"><span data-stu-id="38e1f-124">The id of the role definition.</span></span> |
|<span data-ttu-id="38e1f-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="38e1f-125">resourceId</span></span> |<span data-ttu-id="38e1f-126">String</span><span class="sxs-lookup"><span data-stu-id="38e1f-126">String</span></span>     |<span data-ttu-id="38e1f-127">必須。</span><span class="sxs-lookup"><span data-stu-id="38e1f-127">Required.</span></span> <span data-ttu-id="38e1f-128">ロール定義に関連付けられているリソースの id。</span><span class="sxs-lookup"><span data-stu-id="38e1f-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="38e1f-129">externalId</span><span class="sxs-lookup"><span data-stu-id="38e1f-129">externalId</span></span>   |<span data-ttu-id="38e1f-130">String</span><span class="sxs-lookup"><span data-stu-id="38e1f-130">String</span></span>     |<span data-ttu-id="38e1f-131">ロール定義の外部 id。</span><span class="sxs-lookup"><span data-stu-id="38e1f-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="38e1f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="38e1f-132">displayName</span></span>|<span data-ttu-id="38e1f-133">String</span><span class="sxs-lookup"><span data-stu-id="38e1f-133">String</span></span>     |<span data-ttu-id="38e1f-134">ロール定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="38e1f-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="38e1f-135">templateId</span><span class="sxs-lookup"><span data-stu-id="38e1f-135">templateId</span></span> | <span data-ttu-id="38e1f-136">String</span><span class="sxs-lookup"><span data-stu-id="38e1f-136">String</span></span> | |

## <a name="relationships"></a><span data-ttu-id="38e1f-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="38e1f-137">Relationships</span></span>
| <span data-ttu-id="38e1f-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="38e1f-138">Relationship</span></span> | <span data-ttu-id="38e1f-139">型</span><span class="sxs-lookup"><span data-stu-id="38e1f-139">Type</span></span>   |<span data-ttu-id="38e1f-140">説明</span><span class="sxs-lookup"><span data-stu-id="38e1f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38e1f-141">リソース</span><span class="sxs-lookup"><span data-stu-id="38e1f-141">resource</span></span>|[<span data-ttu-id="38e1f-142">governanceResource</span><span class="sxs-lookup"><span data-stu-id="38e1f-142">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="38e1f-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="38e1f-143">Read-only.</span></span> <span data-ttu-id="38e1f-144">ロール定義に関連付けられているリソース。</span><span class="sxs-lookup"><span data-stu-id="38e1f-144">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="38e1f-145">roleSetting</span><span class="sxs-lookup"><span data-stu-id="38e1f-145">roleSetting</span></span>|[<span data-ttu-id="38e1f-146">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="38e1f-146">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="38e1f-147">ロール定義に関連付けられているロール設定。</span><span class="sxs-lookup"><span data-stu-id="38e1f-147">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38e1f-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38e1f-148">JSON representation</span></span>

<span data-ttu-id="38e1f-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="38e1f-149">Here is a JSON representation of the resource.</span></span>

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
