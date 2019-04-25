---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60fb4f0a782d9502f9e3da3f0a7da2389e937a7d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573418"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="7f025-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f025-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="7f025-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f025-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f025-105">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="7f025-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="7f025-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f025-106">Methods</span></span>
|<span data-ttu-id="7f025-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f025-107">Method</span></span>|<span data-ttu-id="7f025-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f025-108">Return Type</span></span>|<span data-ttu-id="7f025-109">説明</span><span class="sxs-lookup"><span data-stu-id="7f025-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f025-110">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="7f025-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="7f025-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7f025-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7f025-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7f025-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="7f025-113">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="7f025-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="7f025-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7f025-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="7f025-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7f025-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="7f025-116">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="7f025-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="7f025-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7f025-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="7f025-118">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7f025-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="7f025-119">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="7f025-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="7f025-120">なし</span><span class="sxs-lookup"><span data-stu-id="7f025-120">None</span></span>|<span data-ttu-id="7f025-121">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7f025-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="7f025-122">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="7f025-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="7f025-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7f025-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="7f025-124">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f025-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f025-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f025-125">Properties</span></span>
|<span data-ttu-id="7f025-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f025-126">Property</span></span>|<span data-ttu-id="7f025-127">型</span><span class="sxs-lookup"><span data-stu-id="7f025-127">Type</span></span>|<span data-ttu-id="7f025-128">説明</span><span class="sxs-lookup"><span data-stu-id="7f025-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f025-129">id</span><span class="sxs-lookup"><span data-stu-id="7f025-129">id</span></span>|<span data-ttu-id="7f025-130">String</span><span class="sxs-lookup"><span data-stu-id="7f025-130">String</span></span>|<span data-ttu-id="7f025-131">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="7f025-131">The key of the assignment.</span></span>|
|<span data-ttu-id="7f025-132">target</span><span class="sxs-lookup"><span data-stu-id="7f025-132">target</span></span>|[<span data-ttu-id="7f025-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f025-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7f025-134">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="7f025-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f025-135">関係</span><span class="sxs-lookup"><span data-stu-id="7f025-135">Relationships</span></span>
<span data-ttu-id="7f025-136">なし</span><span class="sxs-lookup"><span data-stu-id="7f025-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f025-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f025-137">JSON Representation</span></span>
<span data-ttu-id="7f025-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f025-138">Here is a JSON representation of the resource.</span></span>
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



