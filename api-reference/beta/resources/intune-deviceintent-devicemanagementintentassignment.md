---
title: deviceManagementIntentAssignment リソースの種類
description: インテント割り当てエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c9964e3ef34cc000e102b5ecc253acdb54e92e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371762"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="65350-103">deviceManagementIntentAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65350-103">deviceManagementIntentAssignment resource type</span></span>

> <span data-ttu-id="65350-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65350-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65350-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65350-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65350-106">インテント割り当てエンティティ</span><span class="sxs-lookup"><span data-stu-id="65350-106">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="65350-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="65350-107">Methods</span></span>
|<span data-ttu-id="65350-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="65350-108">Method</span></span>|<span data-ttu-id="65350-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="65350-109">Return Type</span></span>|<span data-ttu-id="65350-110">説明</span><span class="sxs-lookup"><span data-stu-id="65350-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65350-111">DeviceManagementIntentAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="65350-111">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="65350-112">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65350-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="65350-113">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="65350-113">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="65350-114">DeviceManagementIntentAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="65350-114">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="65350-115">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="65350-115">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="65350-116">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="65350-116">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="65350-117">DeviceManagementIntentAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="65350-117">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="65350-118">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="65350-118">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="65350-119">新しい[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="65350-119">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="65350-120">DeviceManagementIntentAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="65350-120">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="65350-121">None</span><span class="sxs-lookup"><span data-stu-id="65350-121">None</span></span>|<span data-ttu-id="65350-122">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="65350-122">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="65350-123">DeviceManagementIntentAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="65350-123">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="65350-124">deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="65350-124">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="65350-125">[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="65350-125">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="65350-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65350-126">Properties</span></span>
|<span data-ttu-id="65350-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65350-127">Property</span></span>|<span data-ttu-id="65350-128">型</span><span class="sxs-lookup"><span data-stu-id="65350-128">Type</span></span>|<span data-ttu-id="65350-129">説明</span><span class="sxs-lookup"><span data-stu-id="65350-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65350-130">id</span><span class="sxs-lookup"><span data-stu-id="65350-130">id</span></span>|<span data-ttu-id="65350-131">String</span><span class="sxs-lookup"><span data-stu-id="65350-131">String</span></span>|<span data-ttu-id="65350-132">割り当て ID</span><span class="sxs-lookup"><span data-stu-id="65350-132">The assignment ID</span></span>|
|<span data-ttu-id="65350-133">target</span><span class="sxs-lookup"><span data-stu-id="65350-133">target</span></span>|[<span data-ttu-id="65350-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="65350-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="65350-135">割り当て先</span><span class="sxs-lookup"><span data-stu-id="65350-135">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="65350-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65350-136">Relationships</span></span>
<span data-ttu-id="65350-137">なし</span><span class="sxs-lookup"><span data-stu-id="65350-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65350-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65350-138">JSON Representation</span></span>
<span data-ttu-id="65350-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65350-139">Here is a JSON representation of the resource.</span></span>
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



