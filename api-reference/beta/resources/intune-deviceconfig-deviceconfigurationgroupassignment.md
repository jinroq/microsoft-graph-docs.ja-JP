---
title: deviceConfigurationGroupAssignment リソースの種類
description: デバイス構成グループの割り当て。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc42e9cf328319e5a6fa2274e091be9a4776a5fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947030"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="703cb-103">deviceConfigurationGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="703cb-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="703cb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="703cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="703cb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="703cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="703cb-106">デバイス構成グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="703cb-106">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="703cb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="703cb-107">Methods</span></span>
|<span data-ttu-id="703cb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="703cb-108">Method</span></span>|<span data-ttu-id="703cb-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="703cb-109">Return Type</span></span>|<span data-ttu-id="703cb-110">説明</span><span class="sxs-lookup"><span data-stu-id="703cb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="703cb-111">リスト deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="703cb-111">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="703cb-112">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="703cb-112">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="703cb-113">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="703cb-113">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="703cb-114">DeviceConfigurationGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="703cb-114">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="703cb-115">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="703cb-115">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="703cb-116">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="703cb-116">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="703cb-117">DeviceConfigurationGroupAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="703cb-117">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="703cb-118">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="703cb-118">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="703cb-119">新しい[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="703cb-119">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="703cb-120">DeviceConfigurationGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="703cb-120">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="703cb-121">None</span><span class="sxs-lookup"><span data-stu-id="703cb-121">None</span></span>|<span data-ttu-id="703cb-122">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="703cb-122">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="703cb-123">DeviceConfigurationGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="703cb-123">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="703cb-124">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="703cb-124">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="703cb-125">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="703cb-125">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="703cb-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="703cb-126">Properties</span></span>
|<span data-ttu-id="703cb-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="703cb-127">Property</span></span>|<span data-ttu-id="703cb-128">種類</span><span class="sxs-lookup"><span data-stu-id="703cb-128">Type</span></span>|<span data-ttu-id="703cb-129">説明</span><span class="sxs-lookup"><span data-stu-id="703cb-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="703cb-130">id</span><span class="sxs-lookup"><span data-stu-id="703cb-130">id</span></span>|<span data-ttu-id="703cb-131">String</span><span class="sxs-lookup"><span data-stu-id="703cb-131">String</span></span>|<span data-ttu-id="703cb-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="703cb-132">Key of the entity.</span></span>|
|<span data-ttu-id="703cb-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="703cb-133">targetGroupId</span></span>|<span data-ttu-id="703cb-134">String</span><span class="sxs-lookup"><span data-stu-id="703cb-134">String</span></span>|<span data-ttu-id="703cb-135">デバイス構成を対象としている AAD グループの Id。</span><span class="sxs-lookup"><span data-stu-id="703cb-135">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="703cb-136">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="703cb-136">excludeGroup</span></span>|<span data-ttu-id="703cb-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="703cb-137">Boolean</span></span>|<span data-ttu-id="703cb-138">このグループを除外する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="703cb-138">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="703cb-139">グループが含まれる既定値</span><span class="sxs-lookup"><span data-stu-id="703cb-139">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="703cb-140">関係</span><span class="sxs-lookup"><span data-stu-id="703cb-140">Relationships</span></span>
|<span data-ttu-id="703cb-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="703cb-141">Relationship</span></span>|<span data-ttu-id="703cb-142">型</span><span class="sxs-lookup"><span data-stu-id="703cb-142">Type</span></span>|<span data-ttu-id="703cb-143">説明</span><span class="sxs-lookup"><span data-stu-id="703cb-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="703cb-144">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="703cb-144">deviceConfiguration</span></span>|[<span data-ttu-id="703cb-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="703cb-145">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="703cb-146">対象とするデバイス構成へのナビゲーションリンク。</span><span class="sxs-lookup"><span data-stu-id="703cb-146">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="703cb-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="703cb-147">JSON Representation</span></span>
<span data-ttu-id="703cb-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="703cb-148">Here is a JSON representation of the resource.</span></span>
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




