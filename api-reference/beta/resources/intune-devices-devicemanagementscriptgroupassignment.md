---
title: devicemanagementscriptgroupassignment リソースの種類
description: グループにデバイス管理スクリプトを割り当てるために使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27028d14289e3e0efdfa705d35d02d67d1fb1835
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154699"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="a4c70-103">devicemanagementscriptgroupassignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4c70-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="a4c70-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4c70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4c70-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4c70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4c70-106">グループにデバイス管理スクリプトを割り当てるために使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a4c70-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="a4c70-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4c70-107">Methods</span></span>
|<span data-ttu-id="a4c70-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4c70-108">Method</span></span>|<span data-ttu-id="a4c70-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a4c70-109">Return Type</span></span>|<span data-ttu-id="a4c70-110">説明</span><span class="sxs-lookup"><span data-stu-id="a4c70-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a4c70-111">devicemanagementscriptgroupassignments の一覧を表示する</span><span class="sxs-lookup"><span data-stu-id="a4c70-111">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="a4c70-112">[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a4c70-112">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="a4c70-113">[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a4c70-113">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="a4c70-114">devicemanagementscriptgroupassignment の取得</span><span class="sxs-lookup"><span data-stu-id="a4c70-114">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="a4c70-115">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a4c70-115">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="a4c70-116">[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a4c70-116">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="a4c70-117">devicemanagementscriptgroupassignment の作成</span><span class="sxs-lookup"><span data-stu-id="a4c70-117">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="a4c70-118">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a4c70-118">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="a4c70-119">新しい[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4c70-119">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="a4c70-120">devicemanagementscriptgroupassignment の削除</span><span class="sxs-lookup"><span data-stu-id="a4c70-120">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="a4c70-121">なし</span><span class="sxs-lookup"><span data-stu-id="a4c70-121">None</span></span>|<span data-ttu-id="a4c70-122">[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a4c70-122">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="a4c70-123">devicemanagementscriptgroupassignment の更新</span><span class="sxs-lookup"><span data-stu-id="a4c70-123">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="a4c70-124">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a4c70-124">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="a4c70-125">[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a4c70-125">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4c70-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4c70-126">Properties</span></span>
|<span data-ttu-id="a4c70-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4c70-127">Property</span></span>|<span data-ttu-id="a4c70-128">型</span><span class="sxs-lookup"><span data-stu-id="a4c70-128">Type</span></span>|<span data-ttu-id="a4c70-129">説明</span><span class="sxs-lookup"><span data-stu-id="a4c70-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4c70-130">id</span><span class="sxs-lookup"><span data-stu-id="a4c70-130">id</span></span>|<span data-ttu-id="a4c70-131">String</span><span class="sxs-lookup"><span data-stu-id="a4c70-131">String</span></span>|<span data-ttu-id="a4c70-132">[デバイス管理スクリプト] グループ割り当てエンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a4c70-132">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="a4c70-133">targetgroupid</span><span class="sxs-lookup"><span data-stu-id="a4c70-133">targetGroupId</span></span>|<span data-ttu-id="a4c70-134">String</span><span class="sxs-lookup"><span data-stu-id="a4c70-134">String</span></span>|<span data-ttu-id="a4c70-135">スクリプトを対象としている Azure Active Directory グループの Id。</span><span class="sxs-lookup"><span data-stu-id="a4c70-135">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4c70-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4c70-136">Relationships</span></span>
<span data-ttu-id="a4c70-137">なし</span><span class="sxs-lookup"><span data-stu-id="a4c70-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4c70-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4c70-138">JSON Representation</span></span>
<span data-ttu-id="a4c70-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4c70-139">Here is a JSON representation of the resource.</span></span>
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




