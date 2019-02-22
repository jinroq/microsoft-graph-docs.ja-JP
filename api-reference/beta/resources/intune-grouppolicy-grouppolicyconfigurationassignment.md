---
title: grouppolicyconfigurationassignment リソースの種類
description: グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d928ff8d65eaf2fb766e579828e2ec7d9b56f05
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160838"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="6d118-103">grouppolicyconfigurationassignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d118-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="6d118-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d118-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d118-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d118-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d118-106">グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="6d118-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="6d118-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d118-107">Methods</span></span>
|<span data-ttu-id="6d118-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d118-108">Method</span></span>|<span data-ttu-id="6d118-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6d118-109">Return Type</span></span>|<span data-ttu-id="6d118-110">説明</span><span class="sxs-lookup"><span data-stu-id="6d118-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6d118-111">grouppolicyconfigurationassignments のリスト</span><span class="sxs-lookup"><span data-stu-id="6d118-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="6d118-112">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6d118-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6d118-113">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6d118-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="6d118-114">grouppolicyconfigurationassignment の取得</span><span class="sxs-lookup"><span data-stu-id="6d118-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="6d118-115">grouppolicyconfigurationassignment</span><span class="sxs-lookup"><span data-stu-id="6d118-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="6d118-116">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6d118-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="6d118-117">grouppolicyconfigurationassignment の作成</span><span class="sxs-lookup"><span data-stu-id="6d118-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="6d118-118">grouppolicyconfigurationassignment</span><span class="sxs-lookup"><span data-stu-id="6d118-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="6d118-119">新しい[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d118-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="6d118-120">grouppolicyconfigurationassignment の削除</span><span class="sxs-lookup"><span data-stu-id="6d118-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="6d118-121">なし</span><span class="sxs-lookup"><span data-stu-id="6d118-121">None</span></span>|<span data-ttu-id="6d118-122">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6d118-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="6d118-123">grouppolicyconfigurationassignment の更新</span><span class="sxs-lookup"><span data-stu-id="6d118-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="6d118-124">grouppolicyconfigurationassignment</span><span class="sxs-lookup"><span data-stu-id="6d118-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="6d118-125">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6d118-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d118-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d118-126">Properties</span></span>
|<span data-ttu-id="6d118-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d118-127">Property</span></span>|<span data-ttu-id="6d118-128">型</span><span class="sxs-lookup"><span data-stu-id="6d118-128">Type</span></span>|<span data-ttu-id="6d118-129">説明</span><span class="sxs-lookup"><span data-stu-id="6d118-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d118-130">id</span><span class="sxs-lookup"><span data-stu-id="6d118-130">id</span></span>|<span data-ttu-id="6d118-131">String</span><span class="sxs-lookup"><span data-stu-id="6d118-131">String</span></span>|<span data-ttu-id="6d118-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6d118-132">Key of the entity.</span></span>|
|<span data-ttu-id="6d118-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d118-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6d118-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d118-134">DateTimeOffset</span></span>|<span data-ttu-id="6d118-135">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="6d118-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="6d118-136">target</span><span class="sxs-lookup"><span data-stu-id="6d118-136">target</span></span>|[<span data-ttu-id="6d118-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6d118-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6d118-138">グループポリシー構成を対象としたグループの種類。</span><span class="sxs-lookup"><span data-stu-id="6d118-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d118-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d118-139">Relationships</span></span>
<span data-ttu-id="6d118-140">なし</span><span class="sxs-lookup"><span data-stu-id="6d118-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d118-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d118-141">JSON Representation</span></span>
<span data-ttu-id="6d118-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6d118-142">Here is a JSON representation of the resource.</span></span>
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




