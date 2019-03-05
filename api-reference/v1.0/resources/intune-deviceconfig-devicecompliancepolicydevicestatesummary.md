---
title: deviceCompliancePolicyDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c434009d1f34014a36e6871963051773aa2aab5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256876"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="d88be-103">deviceCompliancePolicyDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d88be-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="d88be-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d88be-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d88be-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d88be-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="d88be-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d88be-106">Methods</span></span>
|<span data-ttu-id="d88be-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d88be-107">Method</span></span>|<span data-ttu-id="d88be-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d88be-108">Return Type</span></span>|<span data-ttu-id="d88be-109">説明</span><span class="sxs-lookup"><span data-stu-id="d88be-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d88be-110">deviceCompliancePolicyDeviceStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="d88be-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="d88be-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="d88be-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="d88be-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d88be-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="d88be-113">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d88be-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="d88be-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="d88be-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="d88be-115">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d88be-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d88be-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d88be-116">Properties</span></span>
|<span data-ttu-id="d88be-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d88be-117">Property</span></span>|<span data-ttu-id="d88be-118">型</span><span class="sxs-lookup"><span data-stu-id="d88be-118">Type</span></span>|<span data-ttu-id="d88be-119">説明</span><span class="sxs-lookup"><span data-stu-id="d88be-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d88be-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="d88be-120">inGracePeriodCount</span></span>|<span data-ttu-id="d88be-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-121">Int32</span></span>|<span data-ttu-id="d88be-122">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="d88be-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="d88be-123">configManagerCount</span></span>|<span data-ttu-id="d88be-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-124">Int32</span></span>|<span data-ttu-id="d88be-125">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="d88be-126">id</span><span class="sxs-lookup"><span data-stu-id="d88be-126">id</span></span>|<span data-ttu-id="d88be-127">String</span><span class="sxs-lookup"><span data-stu-id="d88be-127">String</span></span>|<span data-ttu-id="d88be-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d88be-128">Key of the entity.</span></span>|
|<span data-ttu-id="d88be-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d88be-129">unknownDeviceCount</span></span>|<span data-ttu-id="d88be-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-130">Int32</span></span>|<span data-ttu-id="d88be-131">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-131">Number of unknown devices</span></span>|
|<span data-ttu-id="d88be-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d88be-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="d88be-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-133">Int32</span></span>|<span data-ttu-id="d88be-134">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="d88be-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d88be-135">compliantDeviceCount</span></span>|<span data-ttu-id="d88be-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-136">Int32</span></span>|<span data-ttu-id="d88be-137">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-137">Number of compliant devices</span></span>|
|<span data-ttu-id="d88be-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d88be-138">remediatedDeviceCount</span></span>|<span data-ttu-id="d88be-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-139">Int32</span></span>|<span data-ttu-id="d88be-140">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-140">Number of remediated devices</span></span>|
|<span data-ttu-id="d88be-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d88be-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d88be-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-142">Int32</span></span>|<span data-ttu-id="d88be-143">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d88be-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d88be-144">errorDeviceCount</span></span>|<span data-ttu-id="d88be-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-145">Int32</span></span>|<span data-ttu-id="d88be-146">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-146">Number of error devices</span></span>|
|<span data-ttu-id="d88be-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d88be-147">conflictDeviceCount</span></span>|<span data-ttu-id="d88be-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d88be-148">Int32</span></span>|<span data-ttu-id="d88be-149">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d88be-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="d88be-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d88be-150">Relationships</span></span>
<span data-ttu-id="d88be-151">なし</span><span class="sxs-lookup"><span data-stu-id="d88be-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d88be-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d88be-152">JSON Representation</span></span>
<span data-ttu-id="d88be-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d88be-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



