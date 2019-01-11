---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8031566663d9113fa40014bdb7bdd7603d3c6174
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842421"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="9c764-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c764-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="9c764-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c764-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c764-105">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="9c764-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="9c764-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c764-106">Methods</span></span>
|<span data-ttu-id="9c764-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c764-107">Method</span></span>|<span data-ttu-id="9c764-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9c764-108">Return Type</span></span>|<span data-ttu-id="9c764-109">説明</span><span class="sxs-lookup"><span data-stu-id="9c764-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9c764-110">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="9c764-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="9c764-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9c764-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9c764-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9c764-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="9c764-113">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="9c764-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="9c764-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9c764-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="9c764-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9c764-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="9c764-116">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="9c764-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="9c764-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9c764-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="9c764-118">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9c764-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="9c764-119">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="9c764-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="9c764-120">なし</span><span class="sxs-lookup"><span data-stu-id="9c764-120">None</span></span>|<span data-ttu-id="9c764-121">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="9c764-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="9c764-122">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="9c764-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="9c764-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="9c764-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="9c764-124">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9c764-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c764-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c764-125">Properties</span></span>
|<span data-ttu-id="9c764-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c764-126">Property</span></span>|<span data-ttu-id="9c764-127">種類</span><span class="sxs-lookup"><span data-stu-id="9c764-127">Type</span></span>|<span data-ttu-id="9c764-128">説明</span><span class="sxs-lookup"><span data-stu-id="9c764-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c764-129">ID</span><span class="sxs-lookup"><span data-stu-id="9c764-129">id</span></span>|<span data-ttu-id="9c764-130">String</span><span class="sxs-lookup"><span data-stu-id="9c764-130">String</span></span>|<span data-ttu-id="9c764-131">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="9c764-131">The key of the assignment.</span></span>|
|<span data-ttu-id="9c764-132">target</span><span class="sxs-lookup"><span data-stu-id="9c764-132">target</span></span>|[<span data-ttu-id="9c764-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9c764-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9c764-134">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="9c764-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c764-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c764-135">Relationships</span></span>
<span data-ttu-id="9c764-136">なし</span><span class="sxs-lookup"><span data-stu-id="9c764-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c764-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c764-137">JSON Representation</span></span>
<span data-ttu-id="9c764-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9c764-138">Here is a JSON representation of the resource.</span></span>
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



