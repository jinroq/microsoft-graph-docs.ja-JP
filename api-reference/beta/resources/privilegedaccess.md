---
title: privilegedAccess リソースの種類
description: " たとえば、は`privilegedAccess/azureResources` 、Azure リソースへの特権アクセスを管理する PIM を表します。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7f59f8420be6ff97511415e944d154cb5d59950f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965790"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="376ab-103">privilegedAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="376ab-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="376ab-104">特権 Id 管理 (PIM) サービスによって提供される機能のグループを表します。</span><span class="sxs-lookup"><span data-stu-id="376ab-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="376ab-105">PIM が管理`privilegedAccess`するさまざまなプロバイダーを表すさまざまなインスタンス。たとえば、は`privilegedAccess/azureResources` 、Azure リソースへの特権アクセスを管理する PIM を表します。</span><span class="sxs-lookup"><span data-stu-id="376ab-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="376ab-106">`privilegedAccess`現時点では読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="376ab-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="376ab-107">`PATCH` `DELETE` `POST` `PUT`エンティティセットでは、、、、または操作はサポートされていません。 `privilegedAccess`</span><span class="sxs-lookup"><span data-stu-id="376ab-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="376ab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="376ab-108">Properties</span></span>
| <span data-ttu-id="376ab-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="376ab-109">Property</span></span>  | <span data-ttu-id="376ab-110">型</span><span class="sxs-lookup"><span data-stu-id="376ab-110">Type</span></span>      |<span data-ttu-id="376ab-111">説明</span><span class="sxs-lookup"><span data-stu-id="376ab-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="376ab-112">id</span><span class="sxs-lookup"><span data-stu-id="376ab-112">id</span></span>         |<span data-ttu-id="376ab-113">文字列</span><span class="sxs-lookup"><span data-stu-id="376ab-113">String</span></span>     |<span data-ttu-id="376ab-114">PIM によって管理されるプロバイダーの id です。</span><span class="sxs-lookup"><span data-stu-id="376ab-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="376ab-115">displayName</span><span class="sxs-lookup"><span data-stu-id="376ab-115">displayName</span></span>|<span data-ttu-id="376ab-116">String</span><span class="sxs-lookup"><span data-stu-id="376ab-116">String</span></span>     |<span data-ttu-id="376ab-117">PIM によって管理されるプロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="376ab-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="376ab-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="376ab-118">Relationships</span></span>
| <span data-ttu-id="376ab-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="376ab-119">Relationship</span></span>   | <span data-ttu-id="376ab-120">型</span><span class="sxs-lookup"><span data-stu-id="376ab-120">Type</span></span>                                         |<span data-ttu-id="376ab-121">説明</span><span class="sxs-lookup"><span data-stu-id="376ab-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="376ab-122">リソース</span><span class="sxs-lookup"><span data-stu-id="376ab-122">resources</span></span>       |<span data-ttu-id="376ab-123">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="376ab-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="376ab-124">プロバイダーのリソースのコレクション。</span><span class="sxs-lookup"><span data-stu-id="376ab-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="376ab-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="376ab-125">roleAssignments</span></span> |<span data-ttu-id="376ab-126">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="376ab-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="376ab-127">プロバイダーのロール割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="376ab-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="376ab-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="376ab-128">roleDefinitions</span></span> |<span data-ttu-id="376ab-129">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="376ab-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="376ab-130">プロバイダーのロール日のコレクション。</span><span class="sxs-lookup"><span data-stu-id="376ab-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="376ab-131">Rolerequests 要求</span><span class="sxs-lookup"><span data-stu-id="376ab-131">roleAssignmentRequests</span></span> |<span data-ttu-id="376ab-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="376ab-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="376ab-133">プロバイダーのロール割り当て要求のコレクション。</span><span class="sxs-lookup"><span data-stu-id="376ab-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="376ab-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="376ab-134">roleSettings</span></span> |<span data-ttu-id="376ab-135">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="376ab-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="376ab-136">プロバイダーのロール設定のコレクション。</span><span class="sxs-lookup"><span data-stu-id="376ab-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="376ab-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="376ab-137">JSON representation</span></span>

<span data-ttu-id="376ab-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="376ab-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
