---
title: deviceConfigurationGroupAssignment リソースの種類
description: デバイス構成のグループの割り当て。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b670ffd828634e244053b8a83e5f1f05f79ebbe1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883980"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="42862-103">deviceConfigurationGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42862-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="42862-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42862-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42862-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42862-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42862-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="42862-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42862-107">デバイス構成のグループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="42862-107">Device configuration group assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="42862-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="42862-108">Methods</span></span>
|<span data-ttu-id="42862-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="42862-109">Method</span></span>|<span data-ttu-id="42862-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="42862-110">Return Type</span></span>|<span data-ttu-id="42862-111">説明</span><span class="sxs-lookup"><span data-stu-id="42862-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42862-112">リスト deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="42862-112">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="42862-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="42862-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="42862-114">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="42862-114">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="42862-115">DeviceConfigurationGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="42862-115">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="42862-116">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="42862-116">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="42862-117">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42862-117">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="42862-118">DeviceConfigurationGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="42862-118">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="42862-119">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="42862-119">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="42862-120">新しい[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="42862-120">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="42862-121">DeviceConfigurationGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="42862-121">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="42862-122">なし</span><span class="sxs-lookup"><span data-stu-id="42862-122">None</span></span>|<span data-ttu-id="42862-123">の[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="42862-123">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="42862-124">DeviceConfigurationGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="42862-124">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="42862-125">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="42862-125">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="42862-126">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="42862-126">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="42862-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42862-127">Properties</span></span>
|<span data-ttu-id="42862-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42862-128">Property</span></span>|<span data-ttu-id="42862-129">種類</span><span class="sxs-lookup"><span data-stu-id="42862-129">Type</span></span>|<span data-ttu-id="42862-130">説明</span><span class="sxs-lookup"><span data-stu-id="42862-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42862-131">ID</span><span class="sxs-lookup"><span data-stu-id="42862-131">id</span></span>|<span data-ttu-id="42862-132">String</span><span class="sxs-lookup"><span data-stu-id="42862-132">String</span></span>|<span data-ttu-id="42862-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="42862-133">Key of the entity.</span></span>|
|<span data-ttu-id="42862-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="42862-134">targetGroupId</span></span>|<span data-ttu-id="42862-135">String</span><span class="sxs-lookup"><span data-stu-id="42862-135">String</span></span>|<span data-ttu-id="42862-136">AAD グループの Id は、対象としてデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="42862-136">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="42862-137">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="42862-137">excludeGroup</span></span>|<span data-ttu-id="42862-138">ブール型</span><span class="sxs-lookup"><span data-stu-id="42862-138">Boolean</span></span>|<span data-ttu-id="42862-139">かどうかをこのグループを除外するようにします。</span><span class="sxs-lookup"><span data-stu-id="42862-139">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="42862-140">既定のグループが含まれている必要があること</span><span class="sxs-lookup"><span data-stu-id="42862-140">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="42862-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42862-141">Relationships</span></span>
|<span data-ttu-id="42862-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42862-142">Relationship</span></span>|<span data-ttu-id="42862-143">型</span><span class="sxs-lookup"><span data-stu-id="42862-143">Type</span></span>|<span data-ttu-id="42862-144">説明</span><span class="sxs-lookup"><span data-stu-id="42862-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42862-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="42862-145">deviceConfiguration</span></span>|[<span data-ttu-id="42862-146">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="42862-146">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="42862-147">ナビゲーション リンクを対象となるデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="42862-147">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42862-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42862-148">JSON Representation</span></span>
<span data-ttu-id="42862-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42862-149">Here is a JSON representation of the resource.</span></span>
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





