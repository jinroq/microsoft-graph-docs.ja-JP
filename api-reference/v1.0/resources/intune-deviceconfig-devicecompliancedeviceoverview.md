---
title: deviceComplianceDeviceOverview リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 3d4a52274e3cc68fbf98f0950ad2bda3ed04b265
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023967"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="68263-103">deviceComplianceDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68263-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="68263-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68263-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68263-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="68263-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="68263-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="68263-106">Methods</span></span>
|<span data-ttu-id="68263-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="68263-107">Method</span></span>|<span data-ttu-id="68263-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="68263-108">Return Type</span></span>|<span data-ttu-id="68263-109">説明</span><span class="sxs-lookup"><span data-stu-id="68263-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68263-110">Get deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="68263-110">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="68263-111">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="68263-111">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="68263-112">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="68263-112">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="68263-113">Update deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="68263-113">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="68263-114">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="68263-114">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="68263-115">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="68263-115">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="68263-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68263-116">Properties</span></span>
|<span data-ttu-id="68263-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68263-117">Property</span></span>|<span data-ttu-id="68263-118">型</span><span class="sxs-lookup"><span data-stu-id="68263-118">Type</span></span>|<span data-ttu-id="68263-119">説明</span><span class="sxs-lookup"><span data-stu-id="68263-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68263-120">id</span><span class="sxs-lookup"><span data-stu-id="68263-120">id</span></span>|<span data-ttu-id="68263-121">String</span><span class="sxs-lookup"><span data-stu-id="68263-121">String</span></span>|<span data-ttu-id="68263-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="68263-122">Key of the entity.</span></span>|
|<span data-ttu-id="68263-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="68263-123">pendingCount</span></span>|<span data-ttu-id="68263-124">Int32</span><span class="sxs-lookup"><span data-stu-id="68263-124">Int32</span></span>|<span data-ttu-id="68263-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="68263-125">Number of pending devices</span></span>|
|<span data-ttu-id="68263-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="68263-126">notApplicableCount</span></span>|<span data-ttu-id="68263-127">Int32</span><span class="sxs-lookup"><span data-stu-id="68263-127">Int32</span></span>|<span data-ttu-id="68263-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="68263-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="68263-129">successCount</span><span class="sxs-lookup"><span data-stu-id="68263-129">successCount</span></span>|<span data-ttu-id="68263-130">Int32</span><span class="sxs-lookup"><span data-stu-id="68263-130">Int32</span></span>|<span data-ttu-id="68263-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="68263-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="68263-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="68263-132">errorCount</span></span>|<span data-ttu-id="68263-133">Int32</span><span class="sxs-lookup"><span data-stu-id="68263-133">Int32</span></span>|<span data-ttu-id="68263-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="68263-134">Number of error devices</span></span>|
|<span data-ttu-id="68263-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="68263-135">failedCount</span></span>|<span data-ttu-id="68263-136">Int32</span><span class="sxs-lookup"><span data-stu-id="68263-136">Int32</span></span>|<span data-ttu-id="68263-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="68263-137">Number of failed devices</span></span>|
|<span data-ttu-id="68263-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="68263-138">lastUpdateDateTime</span></span>|<span data-ttu-id="68263-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68263-139">DateTimeOffset</span></span>|<span data-ttu-id="68263-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="68263-140">Last update time</span></span>|
|<span data-ttu-id="68263-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="68263-141">configurationVersion</span></span>|<span data-ttu-id="68263-142">Int32</span><span class="sxs-lookup"><span data-stu-id="68263-142">Int32</span></span>|<span data-ttu-id="68263-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="68263-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="68263-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68263-144">Relationships</span></span>
<span data-ttu-id="68263-145">なし</span><span class="sxs-lookup"><span data-stu-id="68263-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68263-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68263-146">JSON Representation</span></span>
<span data-ttu-id="68263-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68263-147">Here is a JSON representation of the resource.</span></span>
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



