---
title: deviceConfigurationDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df2fe41a86906a0dc39cefc173d3cb2f83bb0658
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332989"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="89082-103">deviceConfigurationDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89082-103">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="89082-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89082-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89082-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="89082-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89082-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="89082-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="89082-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="89082-107">Methods</span></span>
|<span data-ttu-id="89082-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="89082-108">Method</span></span>|<span data-ttu-id="89082-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="89082-109">Return Type</span></span>|<span data-ttu-id="89082-110">説明</span><span class="sxs-lookup"><span data-stu-id="89082-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89082-111">Get deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="89082-111">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[<span data-ttu-id="89082-112">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="89082-112">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="89082-113">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="89082-113">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="89082-114">Update deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="89082-114">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[<span data-ttu-id="89082-115">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="89082-115">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="89082-116">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="89082-116">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="89082-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89082-117">Properties</span></span>
|<span data-ttu-id="89082-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89082-118">Property</span></span>|<span data-ttu-id="89082-119">型</span><span class="sxs-lookup"><span data-stu-id="89082-119">Type</span></span>|<span data-ttu-id="89082-120">説明</span><span class="sxs-lookup"><span data-stu-id="89082-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89082-121">id</span><span class="sxs-lookup"><span data-stu-id="89082-121">id</span></span>|<span data-ttu-id="89082-122">String</span><span class="sxs-lookup"><span data-stu-id="89082-122">String</span></span>|<span data-ttu-id="89082-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="89082-123">Key of the entity.</span></span>|
|<span data-ttu-id="89082-124">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89082-124">unknownDeviceCount</span></span>|<span data-ttu-id="89082-125">Int32</span><span class="sxs-lookup"><span data-stu-id="89082-125">Int32</span></span>|<span data-ttu-id="89082-126">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89082-126">Number of unknown devices</span></span>|
|<span data-ttu-id="89082-127">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89082-127">notApplicableDeviceCount</span></span>|<span data-ttu-id="89082-128">Int32</span><span class="sxs-lookup"><span data-stu-id="89082-128">Int32</span></span>|<span data-ttu-id="89082-129">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89082-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="89082-130">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89082-130">compliantDeviceCount</span></span>|<span data-ttu-id="89082-131">Int32</span><span class="sxs-lookup"><span data-stu-id="89082-131">Int32</span></span>|<span data-ttu-id="89082-132">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="89082-132">Number of compliant devices</span></span>|
|<span data-ttu-id="89082-133">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89082-133">remediatedDeviceCount</span></span>|<span data-ttu-id="89082-134">Int32</span><span class="sxs-lookup"><span data-stu-id="89082-134">Int32</span></span>|<span data-ttu-id="89082-135">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89082-135">Number of remediated devices</span></span>|
|<span data-ttu-id="89082-136">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89082-136">nonCompliantDeviceCount</span></span>|<span data-ttu-id="89082-137">Int32</span><span class="sxs-lookup"><span data-stu-id="89082-137">Int32</span></span>|<span data-ttu-id="89082-138">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89082-138">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="89082-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89082-139">errorDeviceCount</span></span>|<span data-ttu-id="89082-140">Int32</span><span class="sxs-lookup"><span data-stu-id="89082-140">Int32</span></span>|<span data-ttu-id="89082-141">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="89082-141">Number of error devices</span></span>|
|<span data-ttu-id="89082-142">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89082-142">conflictDeviceCount</span></span>|<span data-ttu-id="89082-143">Int32</span><span class="sxs-lookup"><span data-stu-id="89082-143">Int32</span></span>|<span data-ttu-id="89082-144">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="89082-144">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="89082-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="89082-145">Relationships</span></span>
<span data-ttu-id="89082-146">なし</span><span class="sxs-lookup"><span data-stu-id="89082-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89082-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89082-147">JSON Representation</span></span>
<span data-ttu-id="89082-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="89082-148">Here is a JSON representation of the resource.</span></span>
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



