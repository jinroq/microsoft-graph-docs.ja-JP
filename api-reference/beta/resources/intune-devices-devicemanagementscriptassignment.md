---
title: deviceManagementScriptAssignment リソースの種類
description: グループにデバイス管理スクリプトを割り当てるために使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11e0efcb3dca1d51ed0a1253b9b7a0d0a077da3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370075"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="067ae-103">deviceManagementScriptAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="067ae-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="067ae-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="067ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="067ae-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="067ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="067ae-106">グループにデバイス管理スクリプトを割り当てるために使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="067ae-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="067ae-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="067ae-107">Methods</span></span>
|<span data-ttu-id="067ae-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="067ae-108">Method</span></span>|<span data-ttu-id="067ae-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="067ae-109">Return Type</span></span>|<span data-ttu-id="067ae-110">説明</span><span class="sxs-lookup"><span data-stu-id="067ae-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="067ae-111">リスト deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="067ae-111">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="067ae-112">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="067ae-112">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="067ae-113">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="067ae-113">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="067ae-114">DeviceManagementScriptAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="067ae-114">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="067ae-115">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="067ae-115">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="067ae-116">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="067ae-116">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="067ae-117">DeviceManagementScriptAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="067ae-117">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="067ae-118">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="067ae-118">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="067ae-119">新しい[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="067ae-119">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="067ae-120">DeviceManagementScriptAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="067ae-120">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="067ae-121">None</span><span class="sxs-lookup"><span data-stu-id="067ae-121">None</span></span>|<span data-ttu-id="067ae-122">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="067ae-122">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="067ae-123">DeviceManagementScriptAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="067ae-123">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="067ae-124">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="067ae-124">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="067ae-125">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="067ae-125">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="067ae-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="067ae-126">Properties</span></span>
|<span data-ttu-id="067ae-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="067ae-127">Property</span></span>|<span data-ttu-id="067ae-128">型</span><span class="sxs-lookup"><span data-stu-id="067ae-128">Type</span></span>|<span data-ttu-id="067ae-129">説明</span><span class="sxs-lookup"><span data-stu-id="067ae-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="067ae-130">id</span><span class="sxs-lookup"><span data-stu-id="067ae-130">id</span></span>|<span data-ttu-id="067ae-131">String</span><span class="sxs-lookup"><span data-stu-id="067ae-131">String</span></span>|<span data-ttu-id="067ae-132">[デバイス管理スクリプト] グループ割り当てエンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="067ae-132">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="067ae-133">target</span><span class="sxs-lookup"><span data-stu-id="067ae-133">target</span></span>|[<span data-ttu-id="067ae-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="067ae-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="067ae-135">スクリプトを対象としている Azure Active Directory グループの Id。</span><span class="sxs-lookup"><span data-stu-id="067ae-135">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="067ae-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="067ae-136">Relationships</span></span>
<span data-ttu-id="067ae-137">なし</span><span class="sxs-lookup"><span data-stu-id="067ae-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="067ae-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="067ae-138">JSON Representation</span></span>
<span data-ttu-id="067ae-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="067ae-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



