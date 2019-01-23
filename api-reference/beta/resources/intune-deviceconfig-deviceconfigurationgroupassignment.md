---
title: deviceConfigurationGroupAssignment リソースの種類
description: デバイス構成のグループの割り当て。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ed94f08fb33fe4a999e71b85808f58853d40cad4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406823"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="53b6d-103">deviceConfigurationGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="53b6d-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="53b6d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="53b6d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53b6d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53b6d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53b6d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53b6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53b6d-107">デバイス構成のグループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="53b6d-107">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="53b6d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="53b6d-108">Methods</span></span>
|<span data-ttu-id="53b6d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="53b6d-109">Method</span></span>|<span data-ttu-id="53b6d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="53b6d-110">Return Type</span></span>|<span data-ttu-id="53b6d-111">説明</span><span class="sxs-lookup"><span data-stu-id="53b6d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53b6d-112">リスト deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="53b6d-112">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="53b6d-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="53b6d-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="53b6d-114">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-114">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="53b6d-115">DeviceConfigurationGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-115">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="53b6d-116">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="53b6d-116">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="53b6d-117">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53b6d-117">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="53b6d-118">DeviceConfigurationGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-118">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="53b6d-119">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="53b6d-119">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="53b6d-120">新しい[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-120">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="53b6d-121">DeviceConfigurationGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-121">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="53b6d-122">なし</span><span class="sxs-lookup"><span data-stu-id="53b6d-122">None</span></span>|<span data-ttu-id="53b6d-123">の[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-123">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="53b6d-124">DeviceConfigurationGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-124">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="53b6d-125">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="53b6d-125">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="53b6d-126">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-126">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="53b6d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53b6d-127">Properties</span></span>
|<span data-ttu-id="53b6d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53b6d-128">Property</span></span>|<span data-ttu-id="53b6d-129">型</span><span class="sxs-lookup"><span data-stu-id="53b6d-129">Type</span></span>|<span data-ttu-id="53b6d-130">説明</span><span class="sxs-lookup"><span data-stu-id="53b6d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b6d-131">id</span><span class="sxs-lookup"><span data-stu-id="53b6d-131">id</span></span>|<span data-ttu-id="53b6d-132">String</span><span class="sxs-lookup"><span data-stu-id="53b6d-132">String</span></span>|<span data-ttu-id="53b6d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="53b6d-133">Key of the entity.</span></span>|
|<span data-ttu-id="53b6d-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="53b6d-134">targetGroupId</span></span>|<span data-ttu-id="53b6d-135">String</span><span class="sxs-lookup"><span data-stu-id="53b6d-135">String</span></span>|<span data-ttu-id="53b6d-136">AAD グループの Id は、対象としてデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-136">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="53b6d-137">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="53b6d-137">excludeGroup</span></span>|<span data-ttu-id="53b6d-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="53b6d-138">Boolean</span></span>|<span data-ttu-id="53b6d-139">かどうかをこのグループを除外するようにします。</span><span class="sxs-lookup"><span data-stu-id="53b6d-139">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="53b6d-140">既定のグループが含まれている必要があること</span><span class="sxs-lookup"><span data-stu-id="53b6d-140">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="53b6d-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="53b6d-141">Relationships</span></span>
|<span data-ttu-id="53b6d-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="53b6d-142">Relationship</span></span>|<span data-ttu-id="53b6d-143">型</span><span class="sxs-lookup"><span data-stu-id="53b6d-143">Type</span></span>|<span data-ttu-id="53b6d-144">説明</span><span class="sxs-lookup"><span data-stu-id="53b6d-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b6d-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="53b6d-145">deviceConfiguration</span></span>|[<span data-ttu-id="53b6d-146">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="53b6d-146">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="53b6d-147">ナビゲーション リンクを対象となるデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="53b6d-147">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53b6d-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="53b6d-148">JSON Representation</span></span>
<span data-ttu-id="53b6d-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="53b6d-149">Here is a JSON representation of the resource.</span></span>
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




