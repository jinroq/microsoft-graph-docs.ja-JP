---
title: deviceManagementIntentAssignment リソースの種類
description: インテント割り当てエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c251d6169a35d0be9040afb9fc23442d24e093fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943551"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="84992-103">deviceManagementIntentAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84992-103">deviceManagementIntentAssignment resource type</span></span>

> <span data-ttu-id="84992-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84992-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84992-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="84992-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84992-106">インテント割り当てエンティティ</span><span class="sxs-lookup"><span data-stu-id="84992-106">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="84992-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="84992-107">Methods</span></span>
|<span data-ttu-id="84992-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="84992-108">Method</span></span>|<span data-ttu-id="84992-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="84992-109">Return Type</span></span>|<span data-ttu-id="84992-110">説明</span><span class="sxs-lookup"><span data-stu-id="84992-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84992-111">DeviceManagementIntentAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="84992-111">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="84992-112">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="84992-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="84992-113">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="84992-113">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="84992-114">DeviceManagementIntentAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="84992-114">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="84992-115">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="84992-115">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="84992-116">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="84992-116">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="84992-117">DeviceManagementIntentAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="84992-117">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="84992-118">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="84992-118">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="84992-119">新しい[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="84992-119">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="84992-120">DeviceManagementIntentAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="84992-120">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="84992-121">None</span><span class="sxs-lookup"><span data-stu-id="84992-121">None</span></span>|<span data-ttu-id="84992-122">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="84992-122">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="84992-123">DeviceManagementIntentAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="84992-123">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="84992-124">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="84992-124">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="84992-125">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="84992-125">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84992-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84992-126">Properties</span></span>
|<span data-ttu-id="84992-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84992-127">Property</span></span>|<span data-ttu-id="84992-128">型</span><span class="sxs-lookup"><span data-stu-id="84992-128">Type</span></span>|<span data-ttu-id="84992-129">説明</span><span class="sxs-lookup"><span data-stu-id="84992-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84992-130">id</span><span class="sxs-lookup"><span data-stu-id="84992-130">id</span></span>|<span data-ttu-id="84992-131">String</span><span class="sxs-lookup"><span data-stu-id="84992-131">String</span></span>|<span data-ttu-id="84992-132">割り当て ID</span><span class="sxs-lookup"><span data-stu-id="84992-132">The assignment ID</span></span>|
|<span data-ttu-id="84992-133">target</span><span class="sxs-lookup"><span data-stu-id="84992-133">target</span></span>|[<span data-ttu-id="84992-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="84992-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="84992-135">割り当て先</span><span class="sxs-lookup"><span data-stu-id="84992-135">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="84992-136">関係</span><span class="sxs-lookup"><span data-stu-id="84992-136">Relationships</span></span>
<span data-ttu-id="84992-137">なし</span><span class="sxs-lookup"><span data-stu-id="84992-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84992-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84992-138">JSON Representation</span></span>
<span data-ttu-id="84992-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84992-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




