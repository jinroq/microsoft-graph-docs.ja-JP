---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4a527f8b9da9f11d521311c54697fd04c4f019
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940912"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="2a490-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a490-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="2a490-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a490-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a490-105">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="2a490-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="2a490-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a490-106">Methods</span></span>
|<span data-ttu-id="2a490-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a490-107">Method</span></span>|<span data-ttu-id="2a490-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2a490-108">Return Type</span></span>|<span data-ttu-id="2a490-109">説明</span><span class="sxs-lookup"><span data-stu-id="2a490-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a490-110">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="2a490-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="2a490-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2a490-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2a490-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2a490-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="2a490-113">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="2a490-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="2a490-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a490-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a490-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2a490-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2a490-116">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="2a490-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="2a490-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a490-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a490-118">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2a490-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2a490-119">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="2a490-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="2a490-120">なし</span><span class="sxs-lookup"><span data-stu-id="2a490-120">None</span></span>|<span data-ttu-id="2a490-121">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="2a490-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="2a490-122">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="2a490-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="2a490-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a490-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a490-124">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2a490-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a490-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a490-125">Properties</span></span>
|<span data-ttu-id="2a490-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a490-126">Property</span></span>|<span data-ttu-id="2a490-127">型</span><span class="sxs-lookup"><span data-stu-id="2a490-127">Type</span></span>|<span data-ttu-id="2a490-128">説明</span><span class="sxs-lookup"><span data-stu-id="2a490-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a490-129">ID</span><span class="sxs-lookup"><span data-stu-id="2a490-129">id</span></span>|<span data-ttu-id="2a490-130">String</span><span class="sxs-lookup"><span data-stu-id="2a490-130">String</span></span>|<span data-ttu-id="2a490-131">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="2a490-131">The key of the assignment.</span></span>|
|<span data-ttu-id="2a490-132">target</span><span class="sxs-lookup"><span data-stu-id="2a490-132">target</span></span>|[<span data-ttu-id="2a490-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a490-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2a490-134">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="2a490-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a490-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a490-135">Relationships</span></span>
<span data-ttu-id="2a490-136">なし</span><span class="sxs-lookup"><span data-stu-id="2a490-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a490-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a490-137">JSON Representation</span></span>
<span data-ttu-id="2a490-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a490-138">Here is a JSON representation of the resource.</span></span>
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



