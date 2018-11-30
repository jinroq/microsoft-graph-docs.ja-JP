---
title: deviceManagementScriptGroupAssignment リソースの種類
description: デバイス管理のスクリプトをグループに割り当てるために使用するプロパティが含まれています。
ms.openlocfilehash: e5128403e239f17cbd450726300da1aef3ada193
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070120"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="814b3-103">deviceManagementScriptGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="814b3-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="814b3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="814b3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="814b3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="814b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="814b3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="814b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="814b3-107">デバイス管理のスクリプトをグループに割り当てるために使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="814b3-107">Contains properties used to assign a device management script to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="814b3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="814b3-108">Methods</span></span>
|<span data-ttu-id="814b3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="814b3-109">Method</span></span>|<span data-ttu-id="814b3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="814b3-110">Return Type</span></span>|<span data-ttu-id="814b3-111">説明</span><span class="sxs-lookup"><span data-stu-id="814b3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="814b3-112">リスト deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="814b3-112">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="814b3-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="814b3-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="814b3-114">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="814b3-114">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="814b3-115">DeviceManagementScriptGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="814b3-115">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="814b3-116">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="814b3-116">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="814b3-117">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="814b3-117">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="814b3-118">DeviceManagementScriptGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="814b3-118">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="814b3-119">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="814b3-119">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="814b3-120">新しい[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="814b3-120">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="814b3-121">DeviceManagementScriptGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="814b3-121">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="814b3-122">なし</span><span class="sxs-lookup"><span data-stu-id="814b3-122">None</span></span>|<span data-ttu-id="814b3-123">の[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="814b3-123">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="814b3-124">DeviceManagementScriptGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="814b3-124">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="814b3-125">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="814b3-125">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="814b3-126">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="814b3-126">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="814b3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="814b3-127">Properties</span></span>
|<span data-ttu-id="814b3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="814b3-128">Property</span></span>|<span data-ttu-id="814b3-129">型</span><span class="sxs-lookup"><span data-stu-id="814b3-129">Type</span></span>|<span data-ttu-id="814b3-130">説明</span><span class="sxs-lookup"><span data-stu-id="814b3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="814b3-131">id</span><span class="sxs-lookup"><span data-stu-id="814b3-131">id</span></span>|<span data-ttu-id="814b3-132">String</span><span class="sxs-lookup"><span data-stu-id="814b3-132">String</span></span>|<span data-ttu-id="814b3-133">デバイス管理スクリプトのグループの割り当てエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="814b3-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="814b3-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="814b3-134">targetGroupId</span></span>|<span data-ttu-id="814b3-135">String</span><span class="sxs-lookup"><span data-stu-id="814b3-135">String</span></span>|<span data-ttu-id="814b3-136">Azure Active Directory グループの Id は、対象としてスクリプトをします。</span><span class="sxs-lookup"><span data-stu-id="814b3-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="814b3-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="814b3-137">Relationships</span></span>
<span data-ttu-id="814b3-138">なし</span><span class="sxs-lookup"><span data-stu-id="814b3-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="814b3-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="814b3-139">JSON Representation</span></span>
<span data-ttu-id="814b3-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="814b3-140">Here is a JSON representation of the resource.</span></span>
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





