---
title: deviceCompliancePolicyDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f1234fba81943d984758cd96a6b9f54480e813b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031746"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="b80e7-103">deviceCompliancePolicyDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b80e7-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="b80e7-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b80e7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b80e7-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b80e7-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="b80e7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b80e7-106">Methods</span></span>
|<span data-ttu-id="b80e7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b80e7-107">Method</span></span>|<span data-ttu-id="b80e7-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b80e7-108">Return Type</span></span>|<span data-ttu-id="b80e7-109">説明</span><span class="sxs-lookup"><span data-stu-id="b80e7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b80e7-110">deviceCompliancePolicyDeviceStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="b80e7-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="b80e7-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b80e7-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="b80e7-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b80e7-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="b80e7-113">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="b80e7-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="b80e7-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b80e7-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="b80e7-115">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b80e7-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b80e7-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b80e7-116">Properties</span></span>
|<span data-ttu-id="b80e7-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b80e7-117">Property</span></span>|<span data-ttu-id="b80e7-118">型</span><span class="sxs-lookup"><span data-stu-id="b80e7-118">Type</span></span>|<span data-ttu-id="b80e7-119">説明</span><span class="sxs-lookup"><span data-stu-id="b80e7-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b80e7-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-120">inGracePeriodCount</span></span>|<span data-ttu-id="b80e7-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-121">Int32</span></span>|<span data-ttu-id="b80e7-122">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="b80e7-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-123">configManagerCount</span></span>|<span data-ttu-id="b80e7-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-124">Int32</span></span>|<span data-ttu-id="b80e7-125">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="b80e7-126">id</span><span class="sxs-lookup"><span data-stu-id="b80e7-126">id</span></span>|<span data-ttu-id="b80e7-127">String</span><span class="sxs-lookup"><span data-stu-id="b80e7-127">String</span></span>|<span data-ttu-id="b80e7-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b80e7-128">Key of the entity.</span></span>|
|<span data-ttu-id="b80e7-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-129">unknownDeviceCount</span></span>|<span data-ttu-id="b80e7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-130">Int32</span></span>|<span data-ttu-id="b80e7-131">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-131">Number of unknown devices</span></span>|
|<span data-ttu-id="b80e7-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="b80e7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-133">Int32</span></span>|<span data-ttu-id="b80e7-134">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="b80e7-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-135">compliantDeviceCount</span></span>|<span data-ttu-id="b80e7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-136">Int32</span></span>|<span data-ttu-id="b80e7-137">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-137">Number of compliant devices</span></span>|
|<span data-ttu-id="b80e7-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-138">remediatedDeviceCount</span></span>|<span data-ttu-id="b80e7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-139">Int32</span></span>|<span data-ttu-id="b80e7-140">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-140">Number of remediated devices</span></span>|
|<span data-ttu-id="b80e7-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b80e7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-142">Int32</span></span>|<span data-ttu-id="b80e7-143">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="b80e7-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-144">errorDeviceCount</span></span>|<span data-ttu-id="b80e7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-145">Int32</span></span>|<span data-ttu-id="b80e7-146">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-146">Number of error devices</span></span>|
|<span data-ttu-id="b80e7-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b80e7-147">conflictDeviceCount</span></span>|<span data-ttu-id="b80e7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b80e7-148">Int32</span></span>|<span data-ttu-id="b80e7-149">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="b80e7-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b80e7-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b80e7-150">Relationships</span></span>
<span data-ttu-id="b80e7-151">なし</span><span class="sxs-lookup"><span data-stu-id="b80e7-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b80e7-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b80e7-152">JSON Representation</span></span>
<span data-ttu-id="b80e7-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b80e7-153">Here is a JSON representation of the resource.</span></span>
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



