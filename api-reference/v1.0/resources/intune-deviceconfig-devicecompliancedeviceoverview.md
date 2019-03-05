---
title: deviceComplianceDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b54c617209c37ec623434fd52f5a5fa03db1256
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252386"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="a65cf-103">deviceComplianceDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a65cf-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="a65cf-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a65cf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a65cf-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a65cf-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="a65cf-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a65cf-106">Methods</span></span>
|<span data-ttu-id="a65cf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a65cf-107">Method</span></span>|<span data-ttu-id="a65cf-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a65cf-108">Return Type</span></span>|<span data-ttu-id="a65cf-109">説明</span><span class="sxs-lookup"><span data-stu-id="a65cf-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a65cf-110">Get deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a65cf-110">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="a65cf-111">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a65cf-111">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="a65cf-112">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a65cf-112">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="a65cf-113">Update deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a65cf-113">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="a65cf-114">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a65cf-114">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="a65cf-115">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a65cf-115">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a65cf-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a65cf-116">Properties</span></span>
|<span data-ttu-id="a65cf-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a65cf-117">Property</span></span>|<span data-ttu-id="a65cf-118">型</span><span class="sxs-lookup"><span data-stu-id="a65cf-118">Type</span></span>|<span data-ttu-id="a65cf-119">説明</span><span class="sxs-lookup"><span data-stu-id="a65cf-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a65cf-120">id</span><span class="sxs-lookup"><span data-stu-id="a65cf-120">id</span></span>|<span data-ttu-id="a65cf-121">String</span><span class="sxs-lookup"><span data-stu-id="a65cf-121">String</span></span>|<span data-ttu-id="a65cf-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a65cf-122">Key of the entity.</span></span>|
|<span data-ttu-id="a65cf-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a65cf-123">pendingCount</span></span>|<span data-ttu-id="a65cf-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a65cf-124">Int32</span></span>|<span data-ttu-id="a65cf-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a65cf-125">Number of pending devices</span></span>|
|<span data-ttu-id="a65cf-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a65cf-126">notApplicableCount</span></span>|<span data-ttu-id="a65cf-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a65cf-127">Int32</span></span>|<span data-ttu-id="a65cf-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a65cf-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="a65cf-129">successCount</span><span class="sxs-lookup"><span data-stu-id="a65cf-129">successCount</span></span>|<span data-ttu-id="a65cf-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a65cf-130">Int32</span></span>|<span data-ttu-id="a65cf-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a65cf-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="a65cf-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="a65cf-132">errorCount</span></span>|<span data-ttu-id="a65cf-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a65cf-133">Int32</span></span>|<span data-ttu-id="a65cf-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="a65cf-134">Number of error devices</span></span>|
|<span data-ttu-id="a65cf-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="a65cf-135">failedCount</span></span>|<span data-ttu-id="a65cf-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a65cf-136">Int32</span></span>|<span data-ttu-id="a65cf-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a65cf-137">Number of failed devices</span></span>|
|<span data-ttu-id="a65cf-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a65cf-138">lastUpdateDateTime</span></span>|<span data-ttu-id="a65cf-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a65cf-139">DateTimeOffset</span></span>|<span data-ttu-id="a65cf-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="a65cf-140">Last update time</span></span>|
|<span data-ttu-id="a65cf-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a65cf-141">configurationVersion</span></span>|<span data-ttu-id="a65cf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a65cf-142">Int32</span></span>|<span data-ttu-id="a65cf-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="a65cf-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="a65cf-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a65cf-144">Relationships</span></span>
<span data-ttu-id="a65cf-145">なし</span><span class="sxs-lookup"><span data-stu-id="a65cf-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a65cf-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a65cf-146">JSON Representation</span></span>
<span data-ttu-id="a65cf-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a65cf-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



