---
title: privilegedAccess リソースの種類
description: " たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。"
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512928"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="2b5a4-103">privilegedAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b5a4-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b5a4-104">特権を持つユーザーの管理 (PIM) サービスによって提供される機能のグループを表します。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="2b5a4-105">別のインスタンスの`privilegedAccess`PIM; によって管理されている別のプロバイダーを表します。たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="2b5a4-106">`privilegedAccess`ここでは、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="2b5a4-107">No `POST`、 `PUT`、 `PATCH`、または`DELETE`の操作はサポートされて、`privilegedAccess`のエンティティ セット。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="2b5a4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b5a4-108">Properties</span></span>
| <span data-ttu-id="2b5a4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b5a4-109">Property</span></span>  | <span data-ttu-id="2b5a4-110">型</span><span class="sxs-lookup"><span data-stu-id="2b5a4-110">Type</span></span>      |<span data-ttu-id="2b5a4-111">説明</span><span class="sxs-lookup"><span data-stu-id="2b5a4-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="2b5a4-112">id</span><span class="sxs-lookup"><span data-stu-id="2b5a4-112">id</span></span>         |<span data-ttu-id="2b5a4-113">String</span><span class="sxs-lookup"><span data-stu-id="2b5a4-113">String</span></span>     |<span data-ttu-id="2b5a4-114">PIM によって管理されているプロバイダーの id。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="2b5a4-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2b5a4-115">displayName</span></span>|<span data-ttu-id="2b5a4-116">String</span><span class="sxs-lookup"><span data-stu-id="2b5a4-116">String</span></span>     |<span data-ttu-id="2b5a4-117">PIM によって管理されているプロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2b5a4-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b5a4-118">Relationships</span></span>
| <span data-ttu-id="2b5a4-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b5a4-119">Relationship</span></span>   | <span data-ttu-id="2b5a4-120">型</span><span class="sxs-lookup"><span data-stu-id="2b5a4-120">Type</span></span>                                         |<span data-ttu-id="2b5a4-121">説明</span><span class="sxs-lookup"><span data-stu-id="2b5a4-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="2b5a4-122">resources</span><span class="sxs-lookup"><span data-stu-id="2b5a4-122">resources</span></span>       |<span data-ttu-id="2b5a4-123">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2b5a4-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="2b5a4-124">プロバイダーのリソースのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="2b5a4-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="2b5a4-125">roleAssignments</span></span> |<span data-ttu-id="2b5a4-126">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2b5a4-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="2b5a4-127">プロバイダーのロールの割り当てのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="2b5a4-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="2b5a4-128">roleDefinitions</span></span> |<span data-ttu-id="2b5a4-129">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2b5a4-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="2b5a4-130">プロバイダーのロール定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="2b5a4-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="2b5a4-131">roleAssignmentRequests</span></span> |<span data-ttu-id="2b5a4-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2b5a4-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="2b5a4-133">プロバイダーの役割の割り当て要求のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="2b5a4-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="2b5a4-134">roleSettings</span></span> |<span data-ttu-id="2b5a4-135">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2b5a4-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="2b5a4-136">プロバイダーのロールの設定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2b5a4-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b5a4-137">JSON representation</span></span>

<span data-ttu-id="2b5a4-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b5a4-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
