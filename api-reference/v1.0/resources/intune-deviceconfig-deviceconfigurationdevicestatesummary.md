---
title: deviceConfigurationDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fa887cd1ac6a4dec3f95037e0fdfdf22ad18ee6e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914704"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="674ac-103">deviceConfigurationDeviceStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="674ac-103">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="674ac-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="674ac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="674ac-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="674ac-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="674ac-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="674ac-106">Methods</span></span>
|<span data-ttu-id="674ac-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="674ac-107">Method</span></span>|<span data-ttu-id="674ac-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="674ac-108">Return Type</span></span>|<span data-ttu-id="674ac-109">説明</span><span class="sxs-lookup"><span data-stu-id="674ac-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="674ac-110">Get deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="674ac-110">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[<span data-ttu-id="674ac-111">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="674ac-111">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="674ac-112">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="674ac-112">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="674ac-113">Update deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="674ac-113">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[<span data-ttu-id="674ac-114">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="674ac-114">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="674ac-115">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="674ac-115">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="674ac-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="674ac-116">Properties</span></span>
|<span data-ttu-id="674ac-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="674ac-117">Property</span></span>|<span data-ttu-id="674ac-118">型</span><span class="sxs-lookup"><span data-stu-id="674ac-118">Type</span></span>|<span data-ttu-id="674ac-119">説明</span><span class="sxs-lookup"><span data-stu-id="674ac-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="674ac-120">ID</span><span class="sxs-lookup"><span data-stu-id="674ac-120">id</span></span>|<span data-ttu-id="674ac-121">String</span><span class="sxs-lookup"><span data-stu-id="674ac-121">String</span></span>|<span data-ttu-id="674ac-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="674ac-122">Key of the entity.</span></span>|
|<span data-ttu-id="674ac-123">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="674ac-123">unknownDeviceCount</span></span>|<span data-ttu-id="674ac-124">Int32</span><span class="sxs-lookup"><span data-stu-id="674ac-124">Int32</span></span>|<span data-ttu-id="674ac-125">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="674ac-125">Number of unknown devices</span></span>|
|<span data-ttu-id="674ac-126">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="674ac-126">notApplicableDeviceCount</span></span>|<span data-ttu-id="674ac-127">Int32</span><span class="sxs-lookup"><span data-stu-id="674ac-127">Int32</span></span>|<span data-ttu-id="674ac-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="674ac-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="674ac-129">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="674ac-129">compliantDeviceCount</span></span>|<span data-ttu-id="674ac-130">Int32</span><span class="sxs-lookup"><span data-stu-id="674ac-130">Int32</span></span>|<span data-ttu-id="674ac-131">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="674ac-131">Number of compliant devices</span></span>|
|<span data-ttu-id="674ac-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="674ac-132">remediatedDeviceCount</span></span>|<span data-ttu-id="674ac-133">Int32</span><span class="sxs-lookup"><span data-stu-id="674ac-133">Int32</span></span>|<span data-ttu-id="674ac-134">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="674ac-134">Number of remediated devices</span></span>|
|<span data-ttu-id="674ac-135">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="674ac-135">nonCompliantDeviceCount</span></span>|<span data-ttu-id="674ac-136">Int32</span><span class="sxs-lookup"><span data-stu-id="674ac-136">Int32</span></span>|<span data-ttu-id="674ac-137">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="674ac-137">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="674ac-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="674ac-138">errorDeviceCount</span></span>|<span data-ttu-id="674ac-139">Int32</span><span class="sxs-lookup"><span data-stu-id="674ac-139">Int32</span></span>|<span data-ttu-id="674ac-140">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="674ac-140">Number of error devices</span></span>|
|<span data-ttu-id="674ac-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="674ac-141">conflictDeviceCount</span></span>|<span data-ttu-id="674ac-142">Int32</span><span class="sxs-lookup"><span data-stu-id="674ac-142">Int32</span></span>|<span data-ttu-id="674ac-143">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="674ac-143">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="674ac-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="674ac-144">Relationships</span></span>
<span data-ttu-id="674ac-145">なし</span><span class="sxs-lookup"><span data-stu-id="674ac-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="674ac-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="674ac-146">JSON Representation</span></span>
<span data-ttu-id="674ac-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="674ac-147">Here is a JSON representation of the resource.</span></span>
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



