---
title: managedDeviceOverview リソースの種類
description: 管理対象デバイスの概要データ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f10e34f8db0a671463740f0cbf42785c09170286
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030738"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="2d5b3-103">managedDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d5b3-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="2d5b3-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d5b3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d5b3-105">管理対象デバイスの概要データ</span><span class="sxs-lookup"><span data-stu-id="2d5b3-105">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="2d5b3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2d5b3-106">Methods</span></span>
|<span data-ttu-id="2d5b3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2d5b3-107">Method</span></span>|<span data-ttu-id="2d5b3-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2d5b3-108">Return Type</span></span>|<span data-ttu-id="2d5b3-109">説明</span><span class="sxs-lookup"><span data-stu-id="2d5b3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2d5b3-110">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2d5b3-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="2d5b3-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2d5b3-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="2d5b3-112">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2d5b3-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="2d5b3-113">Update managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2d5b3-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="2d5b3-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2d5b3-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="2d5b3-115">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2d5b3-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d5b3-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d5b3-116">Properties</span></span>
|<span data-ttu-id="2d5b3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d5b3-117">Property</span></span>|<span data-ttu-id="2d5b3-118">型</span><span class="sxs-lookup"><span data-stu-id="2d5b3-118">Type</span></span>|<span data-ttu-id="2d5b3-119">説明</span><span class="sxs-lookup"><span data-stu-id="2d5b3-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d5b3-120">id</span><span class="sxs-lookup"><span data-stu-id="2d5b3-120">id</span></span>|<span data-ttu-id="2d5b3-121">String</span><span class="sxs-lookup"><span data-stu-id="2d5b3-121">String</span></span>|<span data-ttu-id="2d5b3-122">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="2d5b3-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="2d5b3-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d5b3-123">enrolledDeviceCount</span></span>|<span data-ttu-id="2d5b3-124">Int32</span><span class="sxs-lookup"><span data-stu-id="2d5b3-124">Int32</span></span>|<span data-ttu-id="2d5b3-125">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="2d5b3-125">Total enrolled device count.</span></span> <span data-ttu-id="2d5b3-126">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="2d5b3-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="2d5b3-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="2d5b3-127">mdmEnrolledCount</span></span>|<span data-ttu-id="2d5b3-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2d5b3-128">Int32</span></span>|<span data-ttu-id="2d5b3-129">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2d5b3-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="2d5b3-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d5b3-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="2d5b3-131">Int32</span><span class="sxs-lookup"><span data-stu-id="2d5b3-131">Int32</span></span>|<span data-ttu-id="2d5b3-132">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2d5b3-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="2d5b3-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="2d5b3-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="2d5b3-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="2d5b3-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="2d5b3-135">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="2d5b3-135">Device operating system summary.</span></span>|
|<span data-ttu-id="2d5b3-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="2d5b3-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="2d5b3-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="2d5b3-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="2d5b3-138">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="2d5b3-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d5b3-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d5b3-139">Relationships</span></span>
<span data-ttu-id="2d5b3-140">なし</span><span class="sxs-lookup"><span data-stu-id="2d5b3-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d5b3-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d5b3-141">JSON Representation</span></span>
<span data-ttu-id="2d5b3-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2d5b3-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```



