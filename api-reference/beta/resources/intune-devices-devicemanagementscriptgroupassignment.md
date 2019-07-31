---
title: deviceManagementScriptGroupAssignment リソースの種類
description: グループにデバイス管理スクリプトを割り当てるために使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc5b440fbdf5ca0f6ebb7ef28fbf3e4ce868af63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968450"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="07f57-103">deviceManagementScriptGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="07f57-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="07f57-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07f57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07f57-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="07f57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07f57-106">グループにデバイス管理スクリプトを割り当てるために使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="07f57-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="07f57-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="07f57-107">Methods</span></span>
|<span data-ttu-id="07f57-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="07f57-108">Method</span></span>|<span data-ttu-id="07f57-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="07f57-109">Return Type</span></span>|<span data-ttu-id="07f57-110">説明</span><span class="sxs-lookup"><span data-stu-id="07f57-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07f57-111">DeviceManagementScriptGroupAssignments の一覧を表示する</span><span class="sxs-lookup"><span data-stu-id="07f57-111">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="07f57-112">[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="07f57-112">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="07f57-113">[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="07f57-113">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="07f57-114">DeviceManagementScriptGroupAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="07f57-114">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="07f57-115">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07f57-115">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="07f57-116">[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="07f57-116">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="07f57-117">DeviceManagementScriptGroupAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="07f57-117">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="07f57-118">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07f57-118">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="07f57-119">新しい[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="07f57-119">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="07f57-120">DeviceManagementScriptGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="07f57-120">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="07f57-121">None</span><span class="sxs-lookup"><span data-stu-id="07f57-121">None</span></span>|<span data-ttu-id="07f57-122">[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="07f57-122">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="07f57-123">DeviceManagementScriptGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="07f57-123">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="07f57-124">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="07f57-124">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="07f57-125">[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="07f57-125">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07f57-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07f57-126">Properties</span></span>
|<span data-ttu-id="07f57-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07f57-127">Property</span></span>|<span data-ttu-id="07f57-128">型</span><span class="sxs-lookup"><span data-stu-id="07f57-128">Type</span></span>|<span data-ttu-id="07f57-129">説明</span><span class="sxs-lookup"><span data-stu-id="07f57-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07f57-130">id</span><span class="sxs-lookup"><span data-stu-id="07f57-130">id</span></span>|<span data-ttu-id="07f57-131">String</span><span class="sxs-lookup"><span data-stu-id="07f57-131">String</span></span>|<span data-ttu-id="07f57-132">[デバイス管理スクリプト] グループ割り当てエンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="07f57-132">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="07f57-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="07f57-133">targetGroupId</span></span>|<span data-ttu-id="07f57-134">String</span><span class="sxs-lookup"><span data-stu-id="07f57-134">String</span></span>|<span data-ttu-id="07f57-135">スクリプトを対象としている Azure Active Directory グループの Id。</span><span class="sxs-lookup"><span data-stu-id="07f57-135">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07f57-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07f57-136">Relationships</span></span>
<span data-ttu-id="07f57-137">なし</span><span class="sxs-lookup"><span data-stu-id="07f57-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07f57-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07f57-138">JSON Representation</span></span>
<span data-ttu-id="07f57-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="07f57-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```





