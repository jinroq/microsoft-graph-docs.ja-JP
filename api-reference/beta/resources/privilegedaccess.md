---
title: privilegedAccess リソースの種類
description: " たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。"
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810053"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="f3964-103">privilegedAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3964-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="f3964-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3964-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3964-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3964-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3964-106">特権を持つユーザーの管理 (PIM) サービスによって提供される機能のグループを表します。</span><span class="sxs-lookup"><span data-stu-id="f3964-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="f3964-107">別のインスタンスの`privilegedAccess`PIM; によって管理されている別のプロバイダーを表します。たとえば、 `privilegedAccess/azureResources` Azure のリソースへのアクセス権限を管理する PIM を表します。</span><span class="sxs-lookup"><span data-stu-id="f3964-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="f3964-108">`privilegedAccess`ここでは、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f3964-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="f3964-109">No `POST`、 `PUT`、 `PATCH`、または`DELETE`の操作はサポートされて、`privilegedAccess`のエンティティ セット。</span><span class="sxs-lookup"><span data-stu-id="f3964-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="f3964-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3964-110">Properties</span></span>
| <span data-ttu-id="f3964-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3964-111">Property</span></span>  | <span data-ttu-id="f3964-112">種類</span><span class="sxs-lookup"><span data-stu-id="f3964-112">Type</span></span>      |<span data-ttu-id="f3964-113">説明</span><span class="sxs-lookup"><span data-stu-id="f3964-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="f3964-114">ID</span><span class="sxs-lookup"><span data-stu-id="f3964-114">id</span></span>         |<span data-ttu-id="f3964-115">String</span><span class="sxs-lookup"><span data-stu-id="f3964-115">String</span></span>     |<span data-ttu-id="f3964-116">PIM によって管理されているプロバイダーの id。</span><span class="sxs-lookup"><span data-stu-id="f3964-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="f3964-117">displayName</span><span class="sxs-lookup"><span data-stu-id="f3964-117">displayName</span></span>|<span data-ttu-id="f3964-118">String</span><span class="sxs-lookup"><span data-stu-id="f3964-118">String</span></span>     |<span data-ttu-id="f3964-119">PIM によって管理されているプロバイダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="f3964-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f3964-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3964-120">Relationships</span></span>
| <span data-ttu-id="f3964-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3964-121">Relationship</span></span>   | <span data-ttu-id="f3964-122">型</span><span class="sxs-lookup"><span data-stu-id="f3964-122">Type</span></span>                                         |<span data-ttu-id="f3964-123">説明</span><span class="sxs-lookup"><span data-stu-id="f3964-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="f3964-124">resources</span><span class="sxs-lookup"><span data-stu-id="f3964-124">resources</span></span>       |<span data-ttu-id="f3964-125">[governanceResource](../resources/governanceresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3964-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="f3964-126">プロバイダーのリソースのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f3964-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="f3964-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="f3964-127">roleAssignments</span></span> |<span data-ttu-id="f3964-128">[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3964-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="f3964-129">プロバイダーのロールの割り当てのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f3964-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="f3964-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="f3964-130">roleDefinitions</span></span> |<span data-ttu-id="f3964-131">[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3964-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="f3964-132">プロバイダーのロール定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f3964-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="f3964-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f3964-133">roleAssignmentRequests</span></span> |<span data-ttu-id="f3964-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3964-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="f3964-135">プロバイダーの役割の割り当て要求のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f3964-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="f3964-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="f3964-136">roleSettings</span></span> |<span data-ttu-id="f3964-137">[governanceRoleSetting](../resources/governancerolesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3964-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="f3964-138">プロバイダーのロールの設定のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f3964-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f3964-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3964-139">JSON representation</span></span>

<span data-ttu-id="f3964-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3964-140">Here is a JSON representation of the resource.</span></span>

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
