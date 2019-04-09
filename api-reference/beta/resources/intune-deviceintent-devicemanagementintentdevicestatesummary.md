---
title: deviceManagementIntentDeviceStateSummary リソースの種類
description: 目的のデバイス状態の概要を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e65c798cb6d3a3ca5dd1542296b513360d2b080
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524093"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="b0ab0-103">deviceManagementIntentDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0ab0-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

> <span data-ttu-id="b0ab0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0ab0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0ab0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0ab0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0ab0-106">目的のデバイス状態の概要を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="b0ab0-106">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="b0ab0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0ab0-107">Methods</span></span>
|<span data-ttu-id="b0ab0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0ab0-108">Method</span></span>|<span data-ttu-id="b0ab0-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b0ab0-109">Return Type</span></span>|<span data-ttu-id="b0ab0-110">説明</span><span class="sxs-lookup"><span data-stu-id="b0ab0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0ab0-111">deviceManagementIntentDeviceStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="b0ab0-111">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="b0ab0-112">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b0ab0-112">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="b0ab0-113">[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b0ab0-113">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="b0ab0-114">deviceManagementIntentDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="b0ab0-114">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="b0ab0-115">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b0ab0-115">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="b0ab0-116">[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b0ab0-116">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0ab0-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0ab0-117">Properties</span></span>
|<span data-ttu-id="b0ab0-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0ab0-118">Property</span></span>|<span data-ttu-id="b0ab0-119">型</span><span class="sxs-lookup"><span data-stu-id="b0ab0-119">Type</span></span>|<span data-ttu-id="b0ab0-120">説明</span><span class="sxs-lookup"><span data-stu-id="b0ab0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0ab0-121">id</span><span class="sxs-lookup"><span data-stu-id="b0ab0-121">id</span></span>|<span data-ttu-id="b0ab0-122">String</span><span class="sxs-lookup"><span data-stu-id="b0ab0-122">String</span></span>|<span data-ttu-id="b0ab0-123">ID</span><span class="sxs-lookup"><span data-stu-id="b0ab0-123">The ID</span></span>|
|<span data-ttu-id="b0ab0-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b0ab0-124">conflictCount</span></span>|<span data-ttu-id="b0ab0-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ab0-125">Int32</span></span>|<span data-ttu-id="b0ab0-126">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ab0-126">Number of devices in conflict</span></span>|
|<span data-ttu-id="b0ab0-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="b0ab0-127">errorCount</span></span>|<span data-ttu-id="b0ab0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ab0-128">Int32</span></span>|<span data-ttu-id="b0ab0-129">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ab0-129">Number of error devices</span></span>|
|<span data-ttu-id="b0ab0-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="b0ab0-130">failedCount</span></span>|<span data-ttu-id="b0ab0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ab0-131">Int32</span></span>|<span data-ttu-id="b0ab0-132">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ab0-132">Number of failed devices</span></span>|
|<span data-ttu-id="b0ab0-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b0ab0-133">notApplicableCount</span></span>|<span data-ttu-id="b0ab0-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ab0-134">Int32</span></span>|<span data-ttu-id="b0ab0-135">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ab0-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="b0ab0-136">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="b0ab0-136">notApplicablePlatformCount</span></span>|<span data-ttu-id="b0ab0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ab0-137">Int32</span></span>|<span data-ttu-id="b0ab0-138">プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ab0-138">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="b0ab0-139">successCount</span><span class="sxs-lookup"><span data-stu-id="b0ab0-139">successCount</span></span>|<span data-ttu-id="b0ab0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ab0-140">Int32</span></span>|<span data-ttu-id="b0ab0-141">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ab0-141">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0ab0-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b0ab0-142">Relationships</span></span>
<span data-ttu-id="b0ab0-143">なし</span><span class="sxs-lookup"><span data-stu-id="b0ab0-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0ab0-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0ab0-144">JSON Representation</span></span>
<span data-ttu-id="b0ab0-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0ab0-145">Here is a JSON representation of the resource.</span></span>
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







