---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 882cabab9fdc72c3847d3c29bf022f255c101224
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970459"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="a8aad-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8aad-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="a8aad-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8aad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8aad-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8aad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8aad-106">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="a8aad-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="a8aad-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8aad-107">Methods</span></span>
|<span data-ttu-id="a8aad-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8aad-108">Method</span></span>|<span data-ttu-id="a8aad-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a8aad-109">Return Type</span></span>|<span data-ttu-id="a8aad-110">説明</span><span class="sxs-lookup"><span data-stu-id="a8aad-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8aad-111">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="a8aad-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="a8aad-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a8aad-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a8aad-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a8aad-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="a8aad-114">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="a8aad-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="a8aad-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a8aad-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="a8aad-116">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a8aad-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="a8aad-117">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="a8aad-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="a8aad-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a8aad-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="a8aad-119">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a8aad-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="a8aad-120">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="a8aad-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="a8aad-121">なし</span><span class="sxs-lookup"><span data-stu-id="a8aad-121">None</span></span>|<span data-ttu-id="a8aad-122">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a8aad-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="a8aad-123">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="a8aad-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="a8aad-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a8aad-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="a8aad-125">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a8aad-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8aad-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8aad-126">Properties</span></span>
|<span data-ttu-id="a8aad-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8aad-127">Property</span></span>|<span data-ttu-id="a8aad-128">型</span><span class="sxs-lookup"><span data-stu-id="a8aad-128">Type</span></span>|<span data-ttu-id="a8aad-129">説明</span><span class="sxs-lookup"><span data-stu-id="a8aad-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8aad-130">id</span><span class="sxs-lookup"><span data-stu-id="a8aad-130">id</span></span>|<span data-ttu-id="a8aad-131">String</span><span class="sxs-lookup"><span data-stu-id="a8aad-131">String</span></span>|<span data-ttu-id="a8aad-132">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="a8aad-132">The key of the assignment.</span></span>|
|<span data-ttu-id="a8aad-133">target</span><span class="sxs-lookup"><span data-stu-id="a8aad-133">target</span></span>|[<span data-ttu-id="a8aad-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a8aad-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a8aad-135">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="a8aad-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8aad-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a8aad-136">Relationships</span></span>
<span data-ttu-id="a8aad-137">なし</span><span class="sxs-lookup"><span data-stu-id="a8aad-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8aad-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8aad-138">JSON Representation</span></span>
<span data-ttu-id="a8aad-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a8aad-139">Here is a JSON representation of the resource.</span></span>
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





