---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcd13ad7884e572f60f642c087a30bada7dad7f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031676"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="b8ad5-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8ad5-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="b8ad5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8ad5-105">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="b8ad5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8ad5-106">Methods</span></span>
|<span data-ttu-id="b8ad5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8ad5-107">Method</span></span>|<span data-ttu-id="b8ad5-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8ad5-108">Return Type</span></span>|<span data-ttu-id="b8ad5-109">説明</span><span class="sxs-lookup"><span data-stu-id="b8ad5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8ad5-110">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="b8ad5-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="b8ad5-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8ad5-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b8ad5-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="b8ad5-113">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="b8ad5-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="b8ad5-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b8ad5-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="b8ad5-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b8ad5-116">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="b8ad5-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="b8ad5-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b8ad5-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="b8ad5-118">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b8ad5-119">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="b8ad5-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="b8ad5-120">なし</span><span class="sxs-lookup"><span data-stu-id="b8ad5-120">None</span></span>|<span data-ttu-id="b8ad5-121">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="b8ad5-122">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="b8ad5-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="b8ad5-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b8ad5-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="b8ad5-124">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8ad5-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8ad5-125">Properties</span></span>
|<span data-ttu-id="b8ad5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8ad5-126">Property</span></span>|<span data-ttu-id="b8ad5-127">型</span><span class="sxs-lookup"><span data-stu-id="b8ad5-127">Type</span></span>|<span data-ttu-id="b8ad5-128">説明</span><span class="sxs-lookup"><span data-stu-id="b8ad5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ad5-129">id</span><span class="sxs-lookup"><span data-stu-id="b8ad5-129">id</span></span>|<span data-ttu-id="b8ad5-130">String</span><span class="sxs-lookup"><span data-stu-id="b8ad5-130">String</span></span>|<span data-ttu-id="b8ad5-131">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-131">The key of the assignment.</span></span>|
|<span data-ttu-id="b8ad5-132">target</span><span class="sxs-lookup"><span data-stu-id="b8ad5-132">target</span></span>|[<span data-ttu-id="b8ad5-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b8ad5-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b8ad5-134">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8ad5-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8ad5-135">Relationships</span></span>
<span data-ttu-id="b8ad5-136">なし</span><span class="sxs-lookup"><span data-stu-id="b8ad5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8ad5-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8ad5-137">JSON Representation</span></span>
<span data-ttu-id="b8ad5-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8ad5-138">Here is a JSON representation of the resource.</span></span>
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



