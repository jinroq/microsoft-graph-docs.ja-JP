---
title: deviceConfigurationDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13a28f703ffd26d7876c8e9699c7de302f50ade6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150583"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="301ef-103">deviceConfigurationDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="301ef-103">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="301ef-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="301ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="301ef-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="301ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="301ef-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="301ef-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="301ef-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="301ef-107">Methods</span></span>
|<span data-ttu-id="301ef-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="301ef-108">Method</span></span>|<span data-ttu-id="301ef-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="301ef-109">Return Type</span></span>|<span data-ttu-id="301ef-110">説明</span><span class="sxs-lookup"><span data-stu-id="301ef-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="301ef-111">Get deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="301ef-111">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[<span data-ttu-id="301ef-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="301ef-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="301ef-113">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="301ef-113">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="301ef-114">Update deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="301ef-114">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[<span data-ttu-id="301ef-115">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="301ef-115">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="301ef-116">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="301ef-116">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="301ef-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="301ef-117">Properties</span></span>
|<span data-ttu-id="301ef-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="301ef-118">Property</span></span>|<span data-ttu-id="301ef-119">型</span><span class="sxs-lookup"><span data-stu-id="301ef-119">Type</span></span>|<span data-ttu-id="301ef-120">説明</span><span class="sxs-lookup"><span data-stu-id="301ef-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="301ef-121">id</span><span class="sxs-lookup"><span data-stu-id="301ef-121">id</span></span>|<span data-ttu-id="301ef-122">String</span><span class="sxs-lookup"><span data-stu-id="301ef-122">String</span></span>|<span data-ttu-id="301ef-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="301ef-123">Key of the entity.</span></span>|
|<span data-ttu-id="301ef-124">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="301ef-124">unknownDeviceCount</span></span>|<span data-ttu-id="301ef-125">Int32</span><span class="sxs-lookup"><span data-stu-id="301ef-125">Int32</span></span>|<span data-ttu-id="301ef-126">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="301ef-126">Number of unknown devices</span></span>|
|<span data-ttu-id="301ef-127">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="301ef-127">notApplicableDeviceCount</span></span>|<span data-ttu-id="301ef-128">Int32</span><span class="sxs-lookup"><span data-stu-id="301ef-128">Int32</span></span>|<span data-ttu-id="301ef-129">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="301ef-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="301ef-130">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="301ef-130">compliantDeviceCount</span></span>|<span data-ttu-id="301ef-131">Int32</span><span class="sxs-lookup"><span data-stu-id="301ef-131">Int32</span></span>|<span data-ttu-id="301ef-132">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="301ef-132">Number of compliant devices</span></span>|
|<span data-ttu-id="301ef-133">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="301ef-133">remediatedDeviceCount</span></span>|<span data-ttu-id="301ef-134">Int32</span><span class="sxs-lookup"><span data-stu-id="301ef-134">Int32</span></span>|<span data-ttu-id="301ef-135">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="301ef-135">Number of remediated devices</span></span>|
|<span data-ttu-id="301ef-136">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="301ef-136">nonCompliantDeviceCount</span></span>|<span data-ttu-id="301ef-137">Int32</span><span class="sxs-lookup"><span data-stu-id="301ef-137">Int32</span></span>|<span data-ttu-id="301ef-138">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="301ef-138">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="301ef-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="301ef-139">errorDeviceCount</span></span>|<span data-ttu-id="301ef-140">Int32</span><span class="sxs-lookup"><span data-stu-id="301ef-140">Int32</span></span>|<span data-ttu-id="301ef-141">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="301ef-141">Number of error devices</span></span>|
|<span data-ttu-id="301ef-142">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="301ef-142">conflictDeviceCount</span></span>|<span data-ttu-id="301ef-143">Int32</span><span class="sxs-lookup"><span data-stu-id="301ef-143">Int32</span></span>|<span data-ttu-id="301ef-144">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="301ef-144">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="301ef-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="301ef-145">Relationships</span></span>
<span data-ttu-id="301ef-146">なし</span><span class="sxs-lookup"><span data-stu-id="301ef-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="301ef-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="301ef-147">JSON Representation</span></span>
<span data-ttu-id="301ef-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="301ef-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
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




