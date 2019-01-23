---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 115cbd779e53f303bdbf95dc28916879726676ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402602"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="663f8-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="663f8-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="663f8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="663f8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="663f8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="663f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="663f8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="663f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="663f8-107">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="663f8-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="663f8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="663f8-108">Methods</span></span>
|<span data-ttu-id="663f8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="663f8-109">Method</span></span>|<span data-ttu-id="663f8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="663f8-110">Return Type</span></span>|<span data-ttu-id="663f8-111">説明</span><span class="sxs-lookup"><span data-stu-id="663f8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="663f8-112">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="663f8-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="663f8-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="663f8-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="663f8-114">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="663f8-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="663f8-115">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="663f8-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="663f8-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="663f8-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="663f8-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="663f8-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="663f8-118">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="663f8-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="663f8-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="663f8-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="663f8-120">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="663f8-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="663f8-121">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="663f8-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="663f8-122">なし</span><span class="sxs-lookup"><span data-stu-id="663f8-122">None</span></span>|<span data-ttu-id="663f8-123">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="663f8-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="663f8-124">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="663f8-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="663f8-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="663f8-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="663f8-126">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="663f8-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="663f8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="663f8-127">Properties</span></span>
|<span data-ttu-id="663f8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="663f8-128">Property</span></span>|<span data-ttu-id="663f8-129">型</span><span class="sxs-lookup"><span data-stu-id="663f8-129">Type</span></span>|<span data-ttu-id="663f8-130">説明</span><span class="sxs-lookup"><span data-stu-id="663f8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="663f8-131">id</span><span class="sxs-lookup"><span data-stu-id="663f8-131">id</span></span>|<span data-ttu-id="663f8-132">String</span><span class="sxs-lookup"><span data-stu-id="663f8-132">String</span></span>|<span data-ttu-id="663f8-133">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="663f8-133">The key of the assignment.</span></span>|
|<span data-ttu-id="663f8-134">target</span><span class="sxs-lookup"><span data-stu-id="663f8-134">target</span></span>|[<span data-ttu-id="663f8-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="663f8-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="663f8-136">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="663f8-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="663f8-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="663f8-137">Relationships</span></span>
<span data-ttu-id="663f8-138">なし</span><span class="sxs-lookup"><span data-stu-id="663f8-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="663f8-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="663f8-139">JSON Representation</span></span>
<span data-ttu-id="663f8-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="663f8-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




