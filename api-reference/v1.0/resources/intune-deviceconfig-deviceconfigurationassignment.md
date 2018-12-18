---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: tfitzmac
ms.openlocfilehash: 26afc67312ab8544b395b5e20b89a01558fc75d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306245"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="8c065-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c065-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="8c065-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c065-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c065-105">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="8c065-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="8c065-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c065-106">Methods</span></span>
|<span data-ttu-id="8c065-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c065-107">Method</span></span>|<span data-ttu-id="8c065-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8c065-108">Return Type</span></span>|<span data-ttu-id="8c065-109">説明</span><span class="sxs-lookup"><span data-stu-id="8c065-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c065-110">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="8c065-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="8c065-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8c065-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8c065-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8c065-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="8c065-113">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="8c065-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="8c065-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8c065-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8c065-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8c065-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8c065-116">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="8c065-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="8c065-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8c065-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8c065-118">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c065-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8c065-119">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="8c065-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="8c065-120">なし</span><span class="sxs-lookup"><span data-stu-id="8c065-120">None</span></span>|<span data-ttu-id="8c065-121">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="8c065-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="8c065-122">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="8c065-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="8c065-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8c065-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8c065-124">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c065-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c065-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c065-125">Properties</span></span>
|<span data-ttu-id="8c065-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c065-126">Property</span></span>|<span data-ttu-id="8c065-127">種類</span><span class="sxs-lookup"><span data-stu-id="8c065-127">Type</span></span>|<span data-ttu-id="8c065-128">説明</span><span class="sxs-lookup"><span data-stu-id="8c065-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c065-129">ID</span><span class="sxs-lookup"><span data-stu-id="8c065-129">id</span></span>|<span data-ttu-id="8c065-130">String</span><span class="sxs-lookup"><span data-stu-id="8c065-130">String</span></span>|<span data-ttu-id="8c065-131">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="8c065-131">The key of the assignment.</span></span>|
|<span data-ttu-id="8c065-132">target</span><span class="sxs-lookup"><span data-stu-id="8c065-132">target</span></span>|[<span data-ttu-id="8c065-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8c065-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8c065-134">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="8c065-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c065-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c065-135">Relationships</span></span>
<span data-ttu-id="8c065-136">なし</span><span class="sxs-lookup"><span data-stu-id="8c065-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c065-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c065-137">JSON Representation</span></span>
<span data-ttu-id="8c065-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c065-138">Here is a JSON representation of the resource.</span></span>
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



