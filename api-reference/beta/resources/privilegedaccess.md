---
title: privilegedAccess リソースの種類
description: " たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。"
ms.openlocfilehash: af109c0cc355bfb282630d21cd02bb463b944f38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074103"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="64862-103">privilegedAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64862-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="64862-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="64862-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64862-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64862-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64862-106">特権を持つユーザーの管理 (PIM) サービスによって提供される機能のグループを表します。</span><span class="sxs-lookup"><span data-stu-id="64862-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="64862-107">別のインスタンスの`privilegedAccess`PIM; によって管理されている別のプロバイダーを表します。たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。</span><span class="sxs-lookup"><span data-stu-id="64862-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="64862-108">`privilegedAccess`ここでは、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="64862-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="64862-109">No `POST`、 `PUT`、 `PATCH`、または`DELETE`の操作はサポートされて、`privilegedAccess`のエンティティ セット。</span><span class="sxs-lookup"><span data-stu-id="64862-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="64862-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64862-110">Properties</span></span>
| <span data-ttu-id="64862-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64862-111">Property</span></span>  | <span data-ttu-id="64862-112">型</span><span class="sxs-lookup"><span data-stu-id="64862-112">Type</span></span>      |<span data-ttu-id="64862-113">説明</span><span class="sxs-lookup"><span data-stu-id="64862-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="64862-114">id</span><span class="sxs-lookup"><span data-stu-id="64862-114">id</span></span>         |<span data-ttu-id="64862-115">String</span><span class="sxs-lookup"><span data-stu-id="64862-115">String</span></span>     |<span data-ttu-id="64862-116">PIM によって管理されているプロバイダーの id。</span><span class="sxs-lookup"><span data-stu-id="64862-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="64862-117">displayName</span><span class="sxs-lookup"><span data-stu-id="64862-117">displayName</span></span>|<span data-ttu-id="64862-118">String</span><span class="sxs-lookup"><span data-stu-id="64862-118">String</span></span>     |<span data-ttu-id="64862-119">PIM によって管理されているプロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="64862-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="64862-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64862-120">Relationships</span></span>
| <span data-ttu-id="64862-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64862-121">Relationship</span></span>   | <span data-ttu-id="64862-122">型</span><span class="sxs-lookup"><span data-stu-id="64862-122">Type</span></span>                                         |<span data-ttu-id="64862-123">説明</span><span class="sxs-lookup"><span data-stu-id="64862-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="64862-124">resources</span><span class="sxs-lookup"><span data-stu-id="64862-124">resources</span></span>       |<span data-ttu-id="64862-125">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="64862-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="64862-126">プロバイダーのリソースのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="64862-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="64862-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="64862-127">roleAssignments</span></span> |<span data-ttu-id="64862-128">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="64862-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="64862-129">プロバイダーのロールの割り当てのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="64862-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="64862-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="64862-130">roleDefinitions</span></span> |<span data-ttu-id="64862-131">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="64862-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="64862-132">プロバイダーのロール定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="64862-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="64862-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="64862-133">roleAssignmentRequests</span></span> |<span data-ttu-id="64862-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="64862-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="64862-135">プロバイダーの役割の割り当て要求のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="64862-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="64862-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="64862-136">roleSettings</span></span> |<span data-ttu-id="64862-137">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="64862-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="64862-138">プロバイダーのロールの設定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="64862-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="64862-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64862-139">JSON representation</span></span>

<span data-ttu-id="64862-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64862-140">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
