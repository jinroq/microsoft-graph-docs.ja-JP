---
title: groupPolicyConfigurationAssignment リソースの種類
description: グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fc8b21bcf59eccee9460f1f39e3353d0a14bfaf4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998675"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="4c2f4-103">groupPolicyConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c2f4-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="4c2f4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c2f4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c2f4-106">グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="4c2f4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c2f4-107">Methods</span></span>
|<span data-ttu-id="4c2f4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c2f4-108">Method</span></span>|<span data-ttu-id="4c2f4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4c2f4-109">Return Type</span></span>|<span data-ttu-id="4c2f4-110">説明</span><span class="sxs-lookup"><span data-stu-id="4c2f4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4c2f4-111">GroupPolicyConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="4c2f4-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="4c2f4-112">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c2f4-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4c2f4-113">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="4c2f4-114">GroupPolicyConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="4c2f4-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="4c2f4-115">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4c2f4-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="4c2f4-116">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="4c2f4-117">GroupPolicyConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="4c2f4-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="4c2f4-118">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4c2f4-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="4c2f4-119">新しい[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="4c2f4-120">GroupPolicyConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="4c2f4-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="4c2f4-121">None</span><span class="sxs-lookup"><span data-stu-id="4c2f4-121">None</span></span>|<span data-ttu-id="4c2f4-122">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="4c2f4-123">GroupPolicyConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="4c2f4-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="4c2f4-124">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4c2f4-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="4c2f4-125">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c2f4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c2f4-126">Properties</span></span>
|<span data-ttu-id="4c2f4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c2f4-127">Property</span></span>|<span data-ttu-id="4c2f4-128">型</span><span class="sxs-lookup"><span data-stu-id="4c2f4-128">Type</span></span>|<span data-ttu-id="4c2f4-129">説明</span><span class="sxs-lookup"><span data-stu-id="4c2f4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c2f4-130">id</span><span class="sxs-lookup"><span data-stu-id="4c2f4-130">id</span></span>|<span data-ttu-id="4c2f4-131">String</span><span class="sxs-lookup"><span data-stu-id="4c2f4-131">String</span></span>|<span data-ttu-id="4c2f4-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-132">Key of the entity.</span></span>|
|<span data-ttu-id="4c2f4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c2f4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4c2f4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c2f4-134">DateTimeOffset</span></span>|<span data-ttu-id="4c2f4-135">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="4c2f4-136">target</span><span class="sxs-lookup"><span data-stu-id="4c2f4-136">target</span></span>|[<span data-ttu-id="4c2f4-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4c2f4-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4c2f4-138">グループポリシー構成を対象としたグループの種類。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c2f4-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c2f4-139">Relationships</span></span>
<span data-ttu-id="4c2f4-140">なし</span><span class="sxs-lookup"><span data-stu-id="4c2f4-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c2f4-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c2f4-141">JSON Representation</span></span>
<span data-ttu-id="4c2f4-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c2f4-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





