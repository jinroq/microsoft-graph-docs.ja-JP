---
title: privilegedAccess リソースの種類
description: " たとえば、は`privilegedAccess/azureResources` 、Azure リソースへの特権アクセスを管理する PIM を表します。"
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563676"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="ef966-103">privilegedAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef966-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef966-104">特権 id 管理 (PIM) サービスによって提供される機能のグループを表します。</span><span class="sxs-lookup"><span data-stu-id="ef966-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="ef966-105">PIM が管理`privilegedAccess`するさまざまなプロバイダーを表すさまざまなインスタンス。たとえば、は`privilegedAccess/azureResources` 、Azure リソースへの特権アクセスを管理する PIM を表します。</span><span class="sxs-lookup"><span data-stu-id="ef966-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="ef966-106">`privilegedAccess`現時点では読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef966-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="ef966-107">`PATCH` `DELETE` `POST` `PUT`エンティティセットでは、、、、または操作はサポートされていません。 `privilegedAccess`</span><span class="sxs-lookup"><span data-stu-id="ef966-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="ef966-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef966-108">Properties</span></span>
| <span data-ttu-id="ef966-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef966-109">Property</span></span>  | <span data-ttu-id="ef966-110">型</span><span class="sxs-lookup"><span data-stu-id="ef966-110">Type</span></span>      |<span data-ttu-id="ef966-111">説明</span><span class="sxs-lookup"><span data-stu-id="ef966-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="ef966-112">id</span><span class="sxs-lookup"><span data-stu-id="ef966-112">id</span></span>         |<span data-ttu-id="ef966-113">String</span><span class="sxs-lookup"><span data-stu-id="ef966-113">String</span></span>     |<span data-ttu-id="ef966-114">PIM によって管理されるプロバイダーの id です。</span><span class="sxs-lookup"><span data-stu-id="ef966-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="ef966-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ef966-115">displayName</span></span>|<span data-ttu-id="ef966-116">String</span><span class="sxs-lookup"><span data-stu-id="ef966-116">String</span></span>     |<span data-ttu-id="ef966-117">PIM によって管理されるプロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ef966-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="ef966-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef966-118">Relationships</span></span>
| <span data-ttu-id="ef966-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef966-119">Relationship</span></span>   | <span data-ttu-id="ef966-120">型</span><span class="sxs-lookup"><span data-stu-id="ef966-120">Type</span></span>                                         |<span data-ttu-id="ef966-121">説明</span><span class="sxs-lookup"><span data-stu-id="ef966-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="ef966-122">リソース</span><span class="sxs-lookup"><span data-stu-id="ef966-122">resources</span></span>       |<span data-ttu-id="ef966-123">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef966-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="ef966-124">プロバイダーのリソースのコレクション。</span><span class="sxs-lookup"><span data-stu-id="ef966-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="ef966-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="ef966-125">roleAssignments</span></span> |<span data-ttu-id="ef966-126">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef966-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="ef966-127">プロバイダーのロール割り当てのコレクション。</span><span class="sxs-lookup"><span data-stu-id="ef966-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="ef966-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="ef966-128">roleDefinitions</span></span> |<span data-ttu-id="ef966-129">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef966-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="ef966-130">プロバイダーのロール日のコレクション。</span><span class="sxs-lookup"><span data-stu-id="ef966-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="ef966-131">rolerequests 要求</span><span class="sxs-lookup"><span data-stu-id="ef966-131">roleAssignmentRequests</span></span> |<span data-ttu-id="ef966-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef966-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="ef966-133">プロバイダーのロール割り当て要求のコレクション。</span><span class="sxs-lookup"><span data-stu-id="ef966-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="ef966-134">rolesettings</span><span class="sxs-lookup"><span data-stu-id="ef966-134">roleSettings</span></span> |<span data-ttu-id="ef966-135">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef966-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="ef966-136">プロバイダーのロール設定のコレクション。</span><span class="sxs-lookup"><span data-stu-id="ef966-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ef966-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef966-137">JSON representation</span></span>

<span data-ttu-id="ef966-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef966-138">Here is a JSON representation of the resource.</span></span>

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
