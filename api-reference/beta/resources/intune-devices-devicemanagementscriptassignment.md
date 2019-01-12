---
title: deviceManagementScriptAssignment リソースの種類
description: デバイス管理のスクリプトをグループに割り当てるために使用するプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d335f31ceed7ca670981e7702b69950b7f5a864a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923895"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="d2dc8-103">deviceManagementScriptAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2dc8-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="d2dc8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2dc8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2dc8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2dc8-107">デバイス管理のスクリプトをグループに割り当てるために使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-107">Contains properties used to assign a device management script to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="d2dc8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2dc8-108">Methods</span></span>
|<span data-ttu-id="d2dc8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2dc8-109">Method</span></span>|<span data-ttu-id="d2dc8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d2dc8-110">Return Type</span></span>|<span data-ttu-id="d2dc8-111">説明</span><span class="sxs-lookup"><span data-stu-id="d2dc8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2dc8-112">リスト deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="d2dc8-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="d2dc8-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d2dc8-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="d2dc8-114">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="d2dc8-115">DeviceManagementScriptAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="d2dc8-116">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2dc8-116">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d2dc8-117">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="d2dc8-118">DeviceManagementScriptAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="d2dc8-119">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2dc8-119">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d2dc8-120">新しい[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="d2dc8-121">DeviceManagementScriptAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="d2dc8-122">なし</span><span class="sxs-lookup"><span data-stu-id="d2dc8-122">None</span></span>|<span data-ttu-id="d2dc8-123">の[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="d2dc8-124">DeviceManagementScriptAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="d2dc8-125">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d2dc8-125">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d2dc8-126">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2dc8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2dc8-127">Properties</span></span>
|<span data-ttu-id="d2dc8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2dc8-128">Property</span></span>|<span data-ttu-id="d2dc8-129">種類</span><span class="sxs-lookup"><span data-stu-id="d2dc8-129">Type</span></span>|<span data-ttu-id="d2dc8-130">説明</span><span class="sxs-lookup"><span data-stu-id="d2dc8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2dc8-131">ID</span><span class="sxs-lookup"><span data-stu-id="d2dc8-131">id</span></span>|<span data-ttu-id="d2dc8-132">String</span><span class="sxs-lookup"><span data-stu-id="d2dc8-132">String</span></span>|<span data-ttu-id="d2dc8-133">デバイス管理スクリプトのグループの割り当てエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="d2dc8-134">ターゲット</span><span class="sxs-lookup"><span data-stu-id="d2dc8-134">target</span></span>|[<span data-ttu-id="d2dc8-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d2dc8-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d2dc8-136">Azure Active Directory グループの Id は、対象としてスクリプトをします。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2dc8-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2dc8-137">Relationships</span></span>
<span data-ttu-id="d2dc8-138">なし</span><span class="sxs-lookup"><span data-stu-id="d2dc8-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2dc8-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2dc8-139">JSON Representation</span></span>
<span data-ttu-id="d2dc8-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2dc8-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





