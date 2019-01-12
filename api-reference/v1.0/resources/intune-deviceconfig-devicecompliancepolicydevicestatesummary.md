---
title: deviceCompliancePolicyDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c3f047f35718c2172ad5d04a17c07ba746012a2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912954"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="c7363-103">deviceCompliancePolicyDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7363-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="c7363-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7363-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7363-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c7363-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="c7363-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7363-106">Methods</span></span>
|<span data-ttu-id="c7363-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7363-107">Method</span></span>|<span data-ttu-id="c7363-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c7363-108">Return Type</span></span>|<span data-ttu-id="c7363-109">説明</span><span class="sxs-lookup"><span data-stu-id="c7363-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7363-110">deviceCompliancePolicyDeviceStateSummary の取得</span><span class="sxs-lookup"><span data-stu-id="c7363-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="c7363-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c7363-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="c7363-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c7363-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="c7363-113">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="c7363-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="c7363-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c7363-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="c7363-115">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c7363-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7363-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7363-116">Properties</span></span>
|<span data-ttu-id="c7363-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7363-117">Property</span></span>|<span data-ttu-id="c7363-118">型</span><span class="sxs-lookup"><span data-stu-id="c7363-118">Type</span></span>|<span data-ttu-id="c7363-119">説明</span><span class="sxs-lookup"><span data-stu-id="c7363-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7363-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="c7363-120">inGracePeriodCount</span></span>|<span data-ttu-id="c7363-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-121">Int32</span></span>|<span data-ttu-id="c7363-122">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="c7363-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="c7363-123">configManagerCount</span></span>|<span data-ttu-id="c7363-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-124">Int32</span></span>|<span data-ttu-id="c7363-125">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="c7363-126">id</span><span class="sxs-lookup"><span data-stu-id="c7363-126">id</span></span>|<span data-ttu-id="c7363-127">String</span><span class="sxs-lookup"><span data-stu-id="c7363-127">String</span></span>|<span data-ttu-id="c7363-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c7363-128">Key of the entity.</span></span>|
|<span data-ttu-id="c7363-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7363-129">unknownDeviceCount</span></span>|<span data-ttu-id="c7363-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-130">Int32</span></span>|<span data-ttu-id="c7363-131">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-131">Number of unknown devices</span></span>|
|<span data-ttu-id="c7363-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7363-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="c7363-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-133">Int32</span></span>|<span data-ttu-id="c7363-134">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="c7363-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7363-135">compliantDeviceCount</span></span>|<span data-ttu-id="c7363-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-136">Int32</span></span>|<span data-ttu-id="c7363-137">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-137">Number of compliant devices</span></span>|
|<span data-ttu-id="c7363-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7363-138">remediatedDeviceCount</span></span>|<span data-ttu-id="c7363-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-139">Int32</span></span>|<span data-ttu-id="c7363-140">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-140">Number of remediated devices</span></span>|
|<span data-ttu-id="c7363-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7363-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c7363-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-142">Int32</span></span>|<span data-ttu-id="c7363-143">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c7363-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7363-144">errorDeviceCount</span></span>|<span data-ttu-id="c7363-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-145">Int32</span></span>|<span data-ttu-id="c7363-146">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-146">Number of error devices</span></span>|
|<span data-ttu-id="c7363-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7363-147">conflictDeviceCount</span></span>|<span data-ttu-id="c7363-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c7363-148">Int32</span></span>|<span data-ttu-id="c7363-149">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="c7363-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7363-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7363-150">Relationships</span></span>
<span data-ttu-id="c7363-151">なし</span><span class="sxs-lookup"><span data-stu-id="c7363-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7363-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7363-152">JSON Representation</span></span>
<span data-ttu-id="c7363-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7363-153">Here is a JSON representation of the resource.</span></span>
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



