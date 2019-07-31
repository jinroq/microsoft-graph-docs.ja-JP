---
title: deviceConfigurationGroupAssignment リソースの種類
description: デバイス構成グループの割り当て。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4340b7d89ce5f29b174861f921a1246ed936691
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970438"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="d6bfd-103">deviceConfigurationGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6bfd-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="d6bfd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6bfd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6bfd-106">デバイス構成グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-106">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="d6bfd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6bfd-107">Methods</span></span>
|<span data-ttu-id="d6bfd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6bfd-108">Method</span></span>|<span data-ttu-id="d6bfd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d6bfd-109">Return Type</span></span>|<span data-ttu-id="d6bfd-110">説明</span><span class="sxs-lookup"><span data-stu-id="d6bfd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6bfd-111">リスト deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="d6bfd-111">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="d6bfd-112">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d6bfd-112">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="d6bfd-113">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-113">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="d6bfd-114">DeviceConfigurationGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="d6bfd-114">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="d6bfd-115">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d6bfd-115">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="d6bfd-116">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-116">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="d6bfd-117">DeviceConfigurationGroupAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="d6bfd-117">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="d6bfd-118">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d6bfd-118">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="d6bfd-119">新しい[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-119">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="d6bfd-120">DeviceConfigurationGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="d6bfd-120">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="d6bfd-121">None</span><span class="sxs-lookup"><span data-stu-id="d6bfd-121">None</span></span>|<span data-ttu-id="d6bfd-122">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-122">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="d6bfd-123">DeviceConfigurationGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="d6bfd-123">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="d6bfd-124">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d6bfd-124">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="d6bfd-125">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-125">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6bfd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6bfd-126">Properties</span></span>
|<span data-ttu-id="d6bfd-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6bfd-127">Property</span></span>|<span data-ttu-id="d6bfd-128">型</span><span class="sxs-lookup"><span data-stu-id="d6bfd-128">Type</span></span>|<span data-ttu-id="d6bfd-129">説明</span><span class="sxs-lookup"><span data-stu-id="d6bfd-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bfd-130">id</span><span class="sxs-lookup"><span data-stu-id="d6bfd-130">id</span></span>|<span data-ttu-id="d6bfd-131">String</span><span class="sxs-lookup"><span data-stu-id="d6bfd-131">String</span></span>|<span data-ttu-id="d6bfd-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-132">Key of the entity.</span></span>|
|<span data-ttu-id="d6bfd-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="d6bfd-133">targetGroupId</span></span>|<span data-ttu-id="d6bfd-134">String</span><span class="sxs-lookup"><span data-stu-id="d6bfd-134">String</span></span>|<span data-ttu-id="d6bfd-135">デバイス構成を対象としている AAD グループの Id。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-135">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="d6bfd-136">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="d6bfd-136">excludeGroup</span></span>|<span data-ttu-id="d6bfd-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6bfd-137">Boolean</span></span>|<span data-ttu-id="d6bfd-138">このグループを除外する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-138">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="d6bfd-139">グループが含まれる既定値</span><span class="sxs-lookup"><span data-stu-id="d6bfd-139">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6bfd-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d6bfd-140">Relationships</span></span>
|<span data-ttu-id="d6bfd-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d6bfd-141">Relationship</span></span>|<span data-ttu-id="d6bfd-142">型</span><span class="sxs-lookup"><span data-stu-id="d6bfd-142">Type</span></span>|<span data-ttu-id="d6bfd-143">説明</span><span class="sxs-lookup"><span data-stu-id="d6bfd-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bfd-144">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6bfd-144">deviceConfiguration</span></span>|[<span data-ttu-id="d6bfd-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6bfd-145">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="d6bfd-146">対象とするデバイス構成へのナビゲーションリンク。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-146">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6bfd-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6bfd-147">JSON Representation</span></span>
<span data-ttu-id="d6bfd-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d6bfd-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String",
  "excludeGroup": true
}
```





