---
title: deviceManagementIntentDeviceStateSummary リソースの種類
description: 目的のデバイス状態の概要を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72ba65c7b23310a6fb3883bd72579ce838471f4f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964095"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="5fbf7-103">deviceManagementIntentDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5fbf7-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

> <span data-ttu-id="5fbf7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fbf7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fbf7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5fbf7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fbf7-106">目的のデバイス状態の概要を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="5fbf7-106">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="5fbf7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5fbf7-107">Methods</span></span>
|<span data-ttu-id="5fbf7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5fbf7-108">Method</span></span>|<span data-ttu-id="5fbf7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5fbf7-109">Return Type</span></span>|<span data-ttu-id="5fbf7-110">説明</span><span class="sxs-lookup"><span data-stu-id="5fbf7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5fbf7-111">DeviceManagementIntentDeviceStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="5fbf7-111">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="5fbf7-112">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fbf7-112">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="5fbf7-113">[DeviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5fbf7-113">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="5fbf7-114">DeviceManagementIntentDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="5fbf7-114">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="5fbf7-115">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="5fbf7-115">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="5fbf7-116">[DeviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5fbf7-116">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5fbf7-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fbf7-117">Properties</span></span>
|<span data-ttu-id="5fbf7-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fbf7-118">Property</span></span>|<span data-ttu-id="5fbf7-119">型</span><span class="sxs-lookup"><span data-stu-id="5fbf7-119">Type</span></span>|<span data-ttu-id="5fbf7-120">説明</span><span class="sxs-lookup"><span data-stu-id="5fbf7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fbf7-121">id</span><span class="sxs-lookup"><span data-stu-id="5fbf7-121">id</span></span>|<span data-ttu-id="5fbf7-122">String</span><span class="sxs-lookup"><span data-stu-id="5fbf7-122">String</span></span>|<span data-ttu-id="5fbf7-123">ID</span><span class="sxs-lookup"><span data-stu-id="5fbf7-123">The ID</span></span>|
|<span data-ttu-id="5fbf7-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="5fbf7-124">conflictCount</span></span>|<span data-ttu-id="5fbf7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbf7-125">Int32</span></span>|<span data-ttu-id="5fbf7-126">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5fbf7-126">Number of devices in conflict</span></span>|
|<span data-ttu-id="5fbf7-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="5fbf7-127">errorCount</span></span>|<span data-ttu-id="5fbf7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbf7-128">Int32</span></span>|<span data-ttu-id="5fbf7-129">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5fbf7-129">Number of error devices</span></span>|
|<span data-ttu-id="5fbf7-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="5fbf7-130">failedCount</span></span>|<span data-ttu-id="5fbf7-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbf7-131">Int32</span></span>|<span data-ttu-id="5fbf7-132">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5fbf7-132">Number of failed devices</span></span>|
|<span data-ttu-id="5fbf7-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="5fbf7-133">notApplicableCount</span></span>|<span data-ttu-id="5fbf7-134">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbf7-134">Int32</span></span>|<span data-ttu-id="5fbf7-135">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5fbf7-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="5fbf7-136">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="5fbf7-136">notApplicablePlatformCount</span></span>|<span data-ttu-id="5fbf7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbf7-137">Int32</span></span>|<span data-ttu-id="5fbf7-138">プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5fbf7-138">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="5fbf7-139">successCount</span><span class="sxs-lookup"><span data-stu-id="5fbf7-139">successCount</span></span>|<span data-ttu-id="5fbf7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbf7-140">Int32</span></span>|<span data-ttu-id="5fbf7-141">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5fbf7-141">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fbf7-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5fbf7-142">Relationships</span></span>
<span data-ttu-id="5fbf7-143">なし</span><span class="sxs-lookup"><span data-stu-id="5fbf7-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fbf7-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5fbf7-144">JSON Representation</span></span>
<span data-ttu-id="5fbf7-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5fbf7-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024
}
```





