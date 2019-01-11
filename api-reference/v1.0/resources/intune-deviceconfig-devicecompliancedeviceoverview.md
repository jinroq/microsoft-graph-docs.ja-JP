---
title: deviceComplianceDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8ee24c421eb962db68754ad05bcd2b966db0563d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830948"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="6dee5-103">deviceComplianceDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6dee5-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="6dee5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6dee5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6dee5-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6dee5-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="6dee5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6dee5-106">Methods</span></span>
|<span data-ttu-id="6dee5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6dee5-107">Method</span></span>|<span data-ttu-id="6dee5-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6dee5-108">Return Type</span></span>|<span data-ttu-id="6dee5-109">説明</span><span class="sxs-lookup"><span data-stu-id="6dee5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6dee5-110">Get deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6dee5-110">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="6dee5-111">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6dee5-111">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="6dee5-112">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6dee5-112">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="6dee5-113">Update deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6dee5-113">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="6dee5-114">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6dee5-114">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="6dee5-115">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6dee5-115">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6dee5-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dee5-116">Properties</span></span>
|<span data-ttu-id="6dee5-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dee5-117">Property</span></span>|<span data-ttu-id="6dee5-118">種類</span><span class="sxs-lookup"><span data-stu-id="6dee5-118">Type</span></span>|<span data-ttu-id="6dee5-119">説明</span><span class="sxs-lookup"><span data-stu-id="6dee5-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dee5-120">ID</span><span class="sxs-lookup"><span data-stu-id="6dee5-120">id</span></span>|<span data-ttu-id="6dee5-121">String</span><span class="sxs-lookup"><span data-stu-id="6dee5-121">String</span></span>|<span data-ttu-id="6dee5-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6dee5-122">Key of the entity.</span></span>|
|<span data-ttu-id="6dee5-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="6dee5-123">pendingCount</span></span>|<span data-ttu-id="6dee5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="6dee5-124">Int32</span></span>|<span data-ttu-id="6dee5-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6dee5-125">Number of pending devices</span></span>|
|<span data-ttu-id="6dee5-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6dee5-126">notApplicableCount</span></span>|<span data-ttu-id="6dee5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6dee5-127">Int32</span></span>|<span data-ttu-id="6dee5-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6dee5-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="6dee5-129">successCount</span><span class="sxs-lookup"><span data-stu-id="6dee5-129">successCount</span></span>|<span data-ttu-id="6dee5-130">Int32</span><span class="sxs-lookup"><span data-stu-id="6dee5-130">Int32</span></span>|<span data-ttu-id="6dee5-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6dee5-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="6dee5-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="6dee5-132">errorCount</span></span>|<span data-ttu-id="6dee5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6dee5-133">Int32</span></span>|<span data-ttu-id="6dee5-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="6dee5-134">Number of error devices</span></span>|
|<span data-ttu-id="6dee5-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="6dee5-135">failedCount</span></span>|<span data-ttu-id="6dee5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6dee5-136">Int32</span></span>|<span data-ttu-id="6dee5-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6dee5-137">Number of failed devices</span></span>|
|<span data-ttu-id="6dee5-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6dee5-138">lastUpdateDateTime</span></span>|<span data-ttu-id="6dee5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dee5-139">DateTimeOffset</span></span>|<span data-ttu-id="6dee5-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="6dee5-140">Last update time</span></span>|
|<span data-ttu-id="6dee5-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="6dee5-141">configurationVersion</span></span>|<span data-ttu-id="6dee5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6dee5-142">Int32</span></span>|<span data-ttu-id="6dee5-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="6dee5-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dee5-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6dee5-144">Relationships</span></span>
<span data-ttu-id="6dee5-145">なし</span><span class="sxs-lookup"><span data-stu-id="6dee5-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6dee5-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6dee5-146">JSON Representation</span></span>
<span data-ttu-id="6dee5-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6dee5-147">Here is a JSON representation of the resource.</span></span>
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



