---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
ms.openlocfilehash: 447f02252eaa5b894d1cbe27f68242acf6b09a35
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069928"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="c8c3e-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8c3e-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="c8c3e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8c3e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8c3e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8c3e-107">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="c8c3e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c8c3e-108">Methods</span></span>
|<span data-ttu-id="c8c3e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c8c3e-109">Method</span></span>|<span data-ttu-id="c8c3e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c8c3e-110">Return Type</span></span>|<span data-ttu-id="c8c3e-111">説明</span><span class="sxs-lookup"><span data-stu-id="c8c3e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8c3e-112">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="c8c3e-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="c8c3e-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c8c3e-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c8c3e-114">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="c8c3e-115">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="c8c3e-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="c8c3e-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c8c3e-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c8c3e-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c8c3e-118">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="c8c3e-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="c8c3e-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c8c3e-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c8c3e-120">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c8c3e-121">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="c8c3e-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="c8c3e-122">なし</span><span class="sxs-lookup"><span data-stu-id="c8c3e-122">None</span></span>|<span data-ttu-id="c8c3e-123">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="c8c3e-124">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="c8c3e-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="c8c3e-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c8c3e-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c8c3e-126">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8c3e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8c3e-127">Properties</span></span>
|<span data-ttu-id="c8c3e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8c3e-128">Property</span></span>|<span data-ttu-id="c8c3e-129">型</span><span class="sxs-lookup"><span data-stu-id="c8c3e-129">Type</span></span>|<span data-ttu-id="c8c3e-130">説明</span><span class="sxs-lookup"><span data-stu-id="c8c3e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8c3e-131">id</span><span class="sxs-lookup"><span data-stu-id="c8c3e-131">id</span></span>|<span data-ttu-id="c8c3e-132">String</span><span class="sxs-lookup"><span data-stu-id="c8c3e-132">String</span></span>|<span data-ttu-id="c8c3e-133">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-133">The key of the assignment.</span></span>|
|<span data-ttu-id="c8c3e-134">target</span><span class="sxs-lookup"><span data-stu-id="c8c3e-134">target</span></span>|[<span data-ttu-id="c8c3e-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c8c3e-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c8c3e-136">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8c3e-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8c3e-137">Relationships</span></span>
<span data-ttu-id="c8c3e-138">なし</span><span class="sxs-lookup"><span data-stu-id="c8c3e-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8c3e-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8c3e-139">JSON Representation</span></span>
<span data-ttu-id="c8c3e-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8c3e-140">Here is a JSON representation of the resource.</span></span>
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





