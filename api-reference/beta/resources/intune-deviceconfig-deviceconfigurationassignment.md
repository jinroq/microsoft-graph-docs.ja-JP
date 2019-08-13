---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba4aae7fb8706996e0d80d3c3a227b99233b792d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333038"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="56c28-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56c28-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="56c28-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56c28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56c28-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="56c28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56c28-106">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="56c28-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="56c28-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="56c28-107">Methods</span></span>
|<span data-ttu-id="56c28-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="56c28-108">Method</span></span>|<span data-ttu-id="56c28-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="56c28-109">Return Type</span></span>|<span data-ttu-id="56c28-110">説明</span><span class="sxs-lookup"><span data-stu-id="56c28-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56c28-111">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="56c28-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="56c28-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="56c28-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="56c28-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="56c28-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="56c28-114">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="56c28-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="56c28-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="56c28-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="56c28-116">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="56c28-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="56c28-117">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="56c28-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="56c28-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="56c28-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="56c28-119">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="56c28-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="56c28-120">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="56c28-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="56c28-121">なし</span><span class="sxs-lookup"><span data-stu-id="56c28-121">None</span></span>|<span data-ttu-id="56c28-122">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="56c28-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="56c28-123">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="56c28-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="56c28-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="56c28-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="56c28-125">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="56c28-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56c28-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56c28-126">Properties</span></span>
|<span data-ttu-id="56c28-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56c28-127">Property</span></span>|<span data-ttu-id="56c28-128">型</span><span class="sxs-lookup"><span data-stu-id="56c28-128">Type</span></span>|<span data-ttu-id="56c28-129">説明</span><span class="sxs-lookup"><span data-stu-id="56c28-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56c28-130">id</span><span class="sxs-lookup"><span data-stu-id="56c28-130">id</span></span>|<span data-ttu-id="56c28-131">String</span><span class="sxs-lookup"><span data-stu-id="56c28-131">String</span></span>|<span data-ttu-id="56c28-132">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="56c28-132">The key of the assignment.</span></span>|
|<span data-ttu-id="56c28-133">target</span><span class="sxs-lookup"><span data-stu-id="56c28-133">target</span></span>|[<span data-ttu-id="56c28-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="56c28-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="56c28-135">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="56c28-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56c28-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="56c28-136">Relationships</span></span>
<span data-ttu-id="56c28-137">なし</span><span class="sxs-lookup"><span data-stu-id="56c28-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56c28-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56c28-138">JSON Representation</span></span>
<span data-ttu-id="56c28-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="56c28-139">Here is a JSON representation of the resource.</span></span>
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



