---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3580454eae767f9a9ca84e3ab196d66fb0c363d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993166"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="5ca55-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ca55-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="5ca55-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ca55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ca55-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ca55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ca55-106">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="5ca55-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="5ca55-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5ca55-107">Methods</span></span>
|<span data-ttu-id="5ca55-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5ca55-108">Method</span></span>|<span data-ttu-id="5ca55-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5ca55-109">Return Type</span></span>|<span data-ttu-id="5ca55-110">説明</span><span class="sxs-lookup"><span data-stu-id="5ca55-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ca55-111">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="5ca55-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="5ca55-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5ca55-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5ca55-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5ca55-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="5ca55-114">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="5ca55-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="5ca55-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5ca55-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="5ca55-116">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5ca55-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="5ca55-117">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="5ca55-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="5ca55-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5ca55-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="5ca55-119">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ca55-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="5ca55-120">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="5ca55-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="5ca55-121">なし</span><span class="sxs-lookup"><span data-stu-id="5ca55-121">None</span></span>|<span data-ttu-id="5ca55-122">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5ca55-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="5ca55-123">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="5ca55-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="5ca55-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5ca55-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="5ca55-125">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5ca55-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ca55-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ca55-126">Properties</span></span>
|<span data-ttu-id="5ca55-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ca55-127">Property</span></span>|<span data-ttu-id="5ca55-128">型</span><span class="sxs-lookup"><span data-stu-id="5ca55-128">Type</span></span>|<span data-ttu-id="5ca55-129">説明</span><span class="sxs-lookup"><span data-stu-id="5ca55-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ca55-130">id</span><span class="sxs-lookup"><span data-stu-id="5ca55-130">id</span></span>|<span data-ttu-id="5ca55-131">String</span><span class="sxs-lookup"><span data-stu-id="5ca55-131">String</span></span>|<span data-ttu-id="5ca55-132">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="5ca55-132">The key of the assignment.</span></span>|
|<span data-ttu-id="5ca55-133">target</span><span class="sxs-lookup"><span data-stu-id="5ca55-133">target</span></span>|[<span data-ttu-id="5ca55-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5ca55-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5ca55-135">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="5ca55-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ca55-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5ca55-136">Relationships</span></span>
<span data-ttu-id="5ca55-137">なし</span><span class="sxs-lookup"><span data-stu-id="5ca55-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ca55-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ca55-138">JSON Representation</span></span>
<span data-ttu-id="5ca55-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5ca55-139">Here is a JSON representation of the resource.</span></span>
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





