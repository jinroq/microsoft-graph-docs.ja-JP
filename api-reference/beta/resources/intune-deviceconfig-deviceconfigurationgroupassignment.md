---
title: deviceConfigurationGroupAssignment リソースの種類
description: デバイス構成のグループの割り当て。
author: tfitzmac
ms.openlocfilehash: 648edd8122c4e14ad06a6e8b19e5fb83a042affa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334637"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="dddbb-103">deviceConfigurationGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dddbb-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="dddbb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dddbb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dddbb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dddbb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dddbb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dddbb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dddbb-107">デバイス構成のグループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="dddbb-107">Device configuration group assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="dddbb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dddbb-108">Methods</span></span>
|<span data-ttu-id="dddbb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="dddbb-109">Method</span></span>|<span data-ttu-id="dddbb-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dddbb-110">Return Type</span></span>|<span data-ttu-id="dddbb-111">説明</span><span class="sxs-lookup"><span data-stu-id="dddbb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dddbb-112">リスト deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="dddbb-112">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="dddbb-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dddbb-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="dddbb-114">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-114">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="dddbb-115">DeviceConfigurationGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-115">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="dddbb-116">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="dddbb-116">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="dddbb-117">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dddbb-117">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="dddbb-118">DeviceConfigurationGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-118">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="dddbb-119">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="dddbb-119">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="dddbb-120">新しい[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-120">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="dddbb-121">DeviceConfigurationGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-121">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="dddbb-122">なし</span><span class="sxs-lookup"><span data-stu-id="dddbb-122">None</span></span>|<span data-ttu-id="dddbb-123">の[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-123">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="dddbb-124">DeviceConfigurationGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-124">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="dddbb-125">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="dddbb-125">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="dddbb-126">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-126">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dddbb-127">Properties</span><span class="sxs-lookup"><span data-stu-id="dddbb-127">Properties</span></span>
|<span data-ttu-id="dddbb-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dddbb-128">Property</span></span>|<span data-ttu-id="dddbb-129">種類</span><span class="sxs-lookup"><span data-stu-id="dddbb-129">Type</span></span>|<span data-ttu-id="dddbb-130">説明</span><span class="sxs-lookup"><span data-stu-id="dddbb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddbb-131">ID</span><span class="sxs-lookup"><span data-stu-id="dddbb-131">id</span></span>|<span data-ttu-id="dddbb-132">String</span><span class="sxs-lookup"><span data-stu-id="dddbb-132">String</span></span>|<span data-ttu-id="dddbb-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dddbb-133">Key of the entity.</span></span>|
|<span data-ttu-id="dddbb-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="dddbb-134">targetGroupId</span></span>|<span data-ttu-id="dddbb-135">String</span><span class="sxs-lookup"><span data-stu-id="dddbb-135">String</span></span>|<span data-ttu-id="dddbb-136">AAD グループの Id は、対象としてデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-136">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="dddbb-137">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="dddbb-137">excludeGroup</span></span>|<span data-ttu-id="dddbb-138">ブール型</span><span class="sxs-lookup"><span data-stu-id="dddbb-138">Boolean</span></span>|<span data-ttu-id="dddbb-139">かどうかをこのグループを除外するようにします。</span><span class="sxs-lookup"><span data-stu-id="dddbb-139">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="dddbb-140">既定のグループが含まれている必要があること</span><span class="sxs-lookup"><span data-stu-id="dddbb-140">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="dddbb-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dddbb-141">Relationships</span></span>
|<span data-ttu-id="dddbb-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dddbb-142">Relationship</span></span>|<span data-ttu-id="dddbb-143">型</span><span class="sxs-lookup"><span data-stu-id="dddbb-143">Type</span></span>|<span data-ttu-id="dddbb-144">説明</span><span class="sxs-lookup"><span data-stu-id="dddbb-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddbb-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dddbb-145">deviceConfiguration</span></span>|[<span data-ttu-id="dddbb-146">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dddbb-146">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="dddbb-147">ナビゲーション リンクを対象となるデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="dddbb-147">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dddbb-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dddbb-148">JSON Representation</span></span>
<span data-ttu-id="dddbb-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dddbb-149">Here is a JSON representation of the resource.</span></span>
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





