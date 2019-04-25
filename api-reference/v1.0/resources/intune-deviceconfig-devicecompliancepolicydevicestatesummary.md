---
title: deviceCompliancePolicyDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c434009d1f34014a36e6871963051773aa2aab5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572445"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="d9197-103">deviceCompliancePolicyDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9197-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="d9197-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9197-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9197-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d9197-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="d9197-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d9197-106">Methods</span></span>
|<span data-ttu-id="d9197-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d9197-107">Method</span></span>|<span data-ttu-id="d9197-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d9197-108">Return Type</span></span>|<span data-ttu-id="d9197-109">説明</span><span class="sxs-lookup"><span data-stu-id="d9197-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9197-110">deviceCompliancePolicyDeviceStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="d9197-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="d9197-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9197-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="d9197-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d9197-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="d9197-113">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d9197-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="d9197-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9197-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="d9197-115">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d9197-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9197-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9197-116">Properties</span></span>
|<span data-ttu-id="d9197-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9197-117">Property</span></span>|<span data-ttu-id="d9197-118">型</span><span class="sxs-lookup"><span data-stu-id="d9197-118">Type</span></span>|<span data-ttu-id="d9197-119">説明</span><span class="sxs-lookup"><span data-stu-id="d9197-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9197-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="d9197-120">inGracePeriodCount</span></span>|<span data-ttu-id="d9197-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-121">Int32</span></span>|<span data-ttu-id="d9197-122">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="d9197-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="d9197-123">configManagerCount</span></span>|<span data-ttu-id="d9197-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-124">Int32</span></span>|<span data-ttu-id="d9197-125">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="d9197-126">id</span><span class="sxs-lookup"><span data-stu-id="d9197-126">id</span></span>|<span data-ttu-id="d9197-127">String</span><span class="sxs-lookup"><span data-stu-id="d9197-127">String</span></span>|<span data-ttu-id="d9197-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d9197-128">Key of the entity.</span></span>|
|<span data-ttu-id="d9197-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9197-129">unknownDeviceCount</span></span>|<span data-ttu-id="d9197-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-130">Int32</span></span>|<span data-ttu-id="d9197-131">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-131">Number of unknown devices</span></span>|
|<span data-ttu-id="d9197-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9197-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="d9197-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-133">Int32</span></span>|<span data-ttu-id="d9197-134">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="d9197-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9197-135">compliantDeviceCount</span></span>|<span data-ttu-id="d9197-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-136">Int32</span></span>|<span data-ttu-id="d9197-137">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-137">Number of compliant devices</span></span>|
|<span data-ttu-id="d9197-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9197-138">remediatedDeviceCount</span></span>|<span data-ttu-id="d9197-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-139">Int32</span></span>|<span data-ttu-id="d9197-140">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-140">Number of remediated devices</span></span>|
|<span data-ttu-id="d9197-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9197-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d9197-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-142">Int32</span></span>|<span data-ttu-id="d9197-143">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d9197-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9197-144">errorDeviceCount</span></span>|<span data-ttu-id="d9197-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-145">Int32</span></span>|<span data-ttu-id="d9197-146">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-146">Number of error devices</span></span>|
|<span data-ttu-id="d9197-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9197-147">conflictDeviceCount</span></span>|<span data-ttu-id="d9197-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d9197-148">Int32</span></span>|<span data-ttu-id="d9197-149">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d9197-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9197-150">関係</span><span class="sxs-lookup"><span data-stu-id="d9197-150">Relationships</span></span>
<span data-ttu-id="d9197-151">なし</span><span class="sxs-lookup"><span data-stu-id="d9197-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9197-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9197-152">JSON Representation</span></span>
<span data-ttu-id="d9197-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d9197-153">Here is a JSON representation of the resource.</span></span>
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



