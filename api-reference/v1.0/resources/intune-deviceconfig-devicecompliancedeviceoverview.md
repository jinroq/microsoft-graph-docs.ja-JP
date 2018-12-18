---
title: deviceComplianceDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: b7384eef7a1a1c9ddf7be8e3be14807c45604593
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334777"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="b119a-103">deviceComplianceDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b119a-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="b119a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b119a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b119a-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b119a-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="b119a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b119a-106">Methods</span></span>
|<span data-ttu-id="b119a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b119a-107">Method</span></span>|<span data-ttu-id="b119a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b119a-108">Return Type</span></span>|<span data-ttu-id="b119a-109">説明</span><span class="sxs-lookup"><span data-stu-id="b119a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b119a-110">Get deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b119a-110">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="b119a-111">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b119a-111">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="b119a-112">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b119a-112">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="b119a-113">Update deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b119a-113">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="b119a-114">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b119a-114">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="b119a-115">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b119a-115">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b119a-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b119a-116">Properties</span></span>
|<span data-ttu-id="b119a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b119a-117">Property</span></span>|<span data-ttu-id="b119a-118">種類</span><span class="sxs-lookup"><span data-stu-id="b119a-118">Type</span></span>|<span data-ttu-id="b119a-119">説明</span><span class="sxs-lookup"><span data-stu-id="b119a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b119a-120">ID</span><span class="sxs-lookup"><span data-stu-id="b119a-120">id</span></span>|<span data-ttu-id="b119a-121">String</span><span class="sxs-lookup"><span data-stu-id="b119a-121">String</span></span>|<span data-ttu-id="b119a-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b119a-122">Key of the entity.</span></span>|
|<span data-ttu-id="b119a-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b119a-123">pendingCount</span></span>|<span data-ttu-id="b119a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b119a-124">Int32</span></span>|<span data-ttu-id="b119a-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b119a-125">Number of pending devices</span></span>|
|<span data-ttu-id="b119a-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b119a-126">notApplicableCount</span></span>|<span data-ttu-id="b119a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="b119a-127">Int32</span></span>|<span data-ttu-id="b119a-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b119a-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="b119a-129">successCount</span><span class="sxs-lookup"><span data-stu-id="b119a-129">successCount</span></span>|<span data-ttu-id="b119a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b119a-130">Int32</span></span>|<span data-ttu-id="b119a-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b119a-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="b119a-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="b119a-132">errorCount</span></span>|<span data-ttu-id="b119a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b119a-133">Int32</span></span>|<span data-ttu-id="b119a-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="b119a-134">Number of error devices</span></span>|
|<span data-ttu-id="b119a-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="b119a-135">failedCount</span></span>|<span data-ttu-id="b119a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b119a-136">Int32</span></span>|<span data-ttu-id="b119a-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b119a-137">Number of failed devices</span></span>|
|<span data-ttu-id="b119a-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b119a-138">lastUpdateDateTime</span></span>|<span data-ttu-id="b119a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b119a-139">DateTimeOffset</span></span>|<span data-ttu-id="b119a-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="b119a-140">Last update time</span></span>|
|<span data-ttu-id="b119a-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b119a-141">configurationVersion</span></span>|<span data-ttu-id="b119a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b119a-142">Int32</span></span>|<span data-ttu-id="b119a-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="b119a-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="b119a-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b119a-144">Relationships</span></span>
<span data-ttu-id="b119a-145">なし</span><span class="sxs-lookup"><span data-stu-id="b119a-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b119a-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b119a-146">JSON Representation</span></span>
<span data-ttu-id="b119a-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b119a-147">Here is a JSON representation of the resource.</span></span>
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



