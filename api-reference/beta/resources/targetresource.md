---
title: targetResource リソースの種類
description: Audit アクティビティに関連付けられているターゲット ・ リソースの種類のコレクションを表します。 各ターゲット リソースの種類は、次の手順は、このリソースからプロパティを継承します。
localization_priority: Normal
ms.openlocfilehash: f86cfe45870292dae93327859c32d38aa2b252fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828680"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="97026-104">targetResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97026-104">targetResource resource type</span></span>
<span data-ttu-id="97026-105">Audit アクティビティに関連付けられているターゲット ・ リソースの種類のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="97026-105">Indicates a collection of  target resource types associated with the audit activity.</span></span> <span data-ttu-id="97026-106">各ターゲット リソースの種類は、次の手順は、このリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="97026-106">Each target resource type will inherit the properties outlined below from this resource.</span></span>


## <a name="properties"></a><span data-ttu-id="97026-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97026-107">Properties</span></span>
| <span data-ttu-id="97026-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97026-108">Property</span></span>     | <span data-ttu-id="97026-109">種類</span><span class="sxs-lookup"><span data-stu-id="97026-109">Type</span></span>   |<span data-ttu-id="97026-110">説明</span><span class="sxs-lookup"><span data-stu-id="97026-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97026-111">displayName</span><span class="sxs-lookup"><span data-stu-id="97026-111">displayName</span></span>|<span data-ttu-id="97026-112">String</span><span class="sxs-lookup"><span data-stu-id="97026-112">String</span></span>|<span data-ttu-id="97026-113">次のターゲット リソースの種類] の下に記載されているリソースの表示名を示します。</span><span class="sxs-lookup"><span data-stu-id="97026-113">Indicates the display name of the resources outlined under Target Resource Types below.</span></span>|
|<span data-ttu-id="97026-114">id</span><span class="sxs-lookup"><span data-stu-id="97026-114">id</span></span>|<span data-ttu-id="97026-115">String</span><span class="sxs-lookup"><span data-stu-id="97026-115">String</span></span>|<span data-ttu-id="97026-116">リソースの一意の Id を示します (例: ユーザー Id、AppId を RoleId。)。</span><span class="sxs-lookup"><span data-stu-id="97026-116">Indicates the Unique Id of the resource (For example: UserId, AppId, RoleId.).</span></span>|
|<span data-ttu-id="97026-117">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="97026-117">modifiedProperties</span></span>|<span data-ttu-id="97026-118">[modifiedProperty](modifiedproperty.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="97026-118">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="97026-119">名前、変更前の値と変更された各属性の新しい値を示します。</span><span class="sxs-lookup"><span data-stu-id="97026-119">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="97026-120">これは、「更新プログラム」のすべてのアクティビティの適用</span><span class="sxs-lookup"><span data-stu-id="97026-120">This is applicable for any "Update" activities</span></span>|

### <a name="target-resource-types"></a><span data-ttu-id="97026-121">ターゲット リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97026-121">Target Resource Types</span></span>

<span data-ttu-id="97026-122">ターゲット リソースの種類は、基になるリソースによって異なります。</span><span class="sxs-lookup"><span data-stu-id="97026-122">The target resource type varies according to the underlying resource:</span></span>

|<span data-ttu-id="97026-123">リソース名</span><span class="sxs-lookup"><span data-stu-id="97026-123">Resource Name</span></span>| <span data-ttu-id="97026-124">リファレンス</span><span class="sxs-lookup"><span data-stu-id="97026-124">Reference</span></span>|
|-------------|----------|
<span data-ttu-id="97026-125">Device</span><span class="sxs-lookup"><span data-stu-id="97026-125">Device</span></span>|[<span data-ttu-id="97026-126">targetResourceDevice</span><span class="sxs-lookup"><span data-stu-id="97026-126">targetResourceDevice</span></span>](targetresourcedevice.md)
<span data-ttu-id="97026-127">ディレクトリ</span><span class="sxs-lookup"><span data-stu-id="97026-127">Directory</span></span>|<span data-ttu-id="97026-128">[targetResourceDirectory](targetresourcedirectory.md]</span><span class="sxs-lookup"><span data-stu-id="97026-128">[targetResourceDirectory](targetresourcedirectory.md]</span></span>
<span data-ttu-id="97026-129">Group</span><span class="sxs-lookup"><span data-stu-id="97026-129">Group</span></span>|[<span data-ttu-id="97026-130">targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="97026-130">targetResourceGroup</span></span>](targetresourcegroup.md)
<span data-ttu-id="97026-131">ポリシー</span><span class="sxs-lookup"><span data-stu-id="97026-131">Policy</span></span>|[<span data-ttu-id="97026-132">targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="97026-132">targetResourcePolicy</span></span>](targetresourcepolicy.md)
<span data-ttu-id="97026-133">Role</span><span class="sxs-lookup"><span data-stu-id="97026-133">Role</span></span>|[<span data-ttu-id="97026-134">targetResourceRole</span><span class="sxs-lookup"><span data-stu-id="97026-134">targetResourceRole</span></span>](targetresourcerole.md)
<span data-ttu-id="97026-135">サービス ・ プリンシパル</span><span class="sxs-lookup"><span data-stu-id="97026-135">Service Principal</span></span>|[<span data-ttu-id="97026-136">targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="97026-136">targetResourceServicePrincipal</span></span>](targetresourceserviceprincipal.md)
<span data-ttu-id="97026-137">User</span><span class="sxs-lookup"><span data-stu-id="97026-137">User</span></span>|[<span data-ttu-id="97026-138">targetResourceUser</span><span class="sxs-lookup"><span data-stu-id="97026-138">targetResourceUser</span></span>](targetresourceuser.md)
<span data-ttu-id="97026-139">その他</span><span class="sxs-lookup"><span data-stu-id="97026-139">Other</span></span>|[<span data-ttu-id="97026-140">targetResourceOther</span><span class="sxs-lookup"><span data-stu-id="97026-140">targetResourceOther</span></span>](targetresourceother.md)

## <a name="json-representation"></a><span data-ttu-id="97026-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97026-141">JSON representation</span></span>

<span data-ttu-id="97026-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97026-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
