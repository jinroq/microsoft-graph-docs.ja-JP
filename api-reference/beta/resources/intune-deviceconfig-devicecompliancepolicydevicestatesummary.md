---
title: deviceCompliancePolicyDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 933f6c10186e2709cdcd2aa388662a609b569e3c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333143"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="18738-103">deviceCompliancePolicyDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18738-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="18738-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18738-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18738-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18738-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18738-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="18738-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="18738-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="18738-107">Methods</span></span>
|<span data-ttu-id="18738-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="18738-108">Method</span></span>|<span data-ttu-id="18738-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="18738-109">Return Type</span></span>|<span data-ttu-id="18738-110">説明</span><span class="sxs-lookup"><span data-stu-id="18738-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18738-111">deviceCompliancePolicyDeviceStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="18738-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="18738-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="18738-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="18738-113">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="18738-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="18738-114">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="18738-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="18738-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="18738-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="18738-116">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="18738-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18738-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18738-117">Properties</span></span>
|<span data-ttu-id="18738-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18738-118">Property</span></span>|<span data-ttu-id="18738-119">型</span><span class="sxs-lookup"><span data-stu-id="18738-119">Type</span></span>|<span data-ttu-id="18738-120">説明</span><span class="sxs-lookup"><span data-stu-id="18738-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18738-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="18738-121">inGracePeriodCount</span></span>|<span data-ttu-id="18738-122">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-122">Int32</span></span>|<span data-ttu-id="18738-123">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="18738-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="18738-124">configManagerCount</span></span>|<span data-ttu-id="18738-125">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-125">Int32</span></span>|<span data-ttu-id="18738-126">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="18738-127">id</span><span class="sxs-lookup"><span data-stu-id="18738-127">id</span></span>|<span data-ttu-id="18738-128">String</span><span class="sxs-lookup"><span data-stu-id="18738-128">String</span></span>|<span data-ttu-id="18738-129">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="18738-129">Key of the entity.</span></span>|
|<span data-ttu-id="18738-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="18738-130">unknownDeviceCount</span></span>|<span data-ttu-id="18738-131">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-131">Int32</span></span>|<span data-ttu-id="18738-132">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-132">Number of unknown devices</span></span>|
|<span data-ttu-id="18738-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="18738-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="18738-134">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-134">Int32</span></span>|<span data-ttu-id="18738-135">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="18738-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="18738-136">compliantDeviceCount</span></span>|<span data-ttu-id="18738-137">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-137">Int32</span></span>|<span data-ttu-id="18738-138">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-138">Number of compliant devices</span></span>|
|<span data-ttu-id="18738-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="18738-139">remediatedDeviceCount</span></span>|<span data-ttu-id="18738-140">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-140">Int32</span></span>|<span data-ttu-id="18738-141">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-141">Number of remediated devices</span></span>|
|<span data-ttu-id="18738-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="18738-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="18738-143">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-143">Int32</span></span>|<span data-ttu-id="18738-144">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="18738-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="18738-145">errorDeviceCount</span></span>|<span data-ttu-id="18738-146">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-146">Int32</span></span>|<span data-ttu-id="18738-147">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-147">Number of error devices</span></span>|
|<span data-ttu-id="18738-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="18738-148">conflictDeviceCount</span></span>|<span data-ttu-id="18738-149">Int32</span><span class="sxs-lookup"><span data-stu-id="18738-149">Int32</span></span>|<span data-ttu-id="18738-150">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="18738-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="18738-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18738-151">Relationships</span></span>
<span data-ttu-id="18738-152">なし</span><span class="sxs-lookup"><span data-stu-id="18738-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18738-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18738-153">JSON Representation</span></span>
<span data-ttu-id="18738-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18738-154">Here is a JSON representation of the resource.</span></span>
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



