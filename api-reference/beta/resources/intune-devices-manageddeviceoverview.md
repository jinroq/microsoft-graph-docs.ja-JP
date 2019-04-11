---
title: managedDeviceOverview リソースの種類
description: 管理対象デバイスの概要データ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07a6bda1e62088eabc3450cf2dcefc945f3ca898
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771202"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="a33c5-103">managedDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a33c5-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="a33c5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a33c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a33c5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a33c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a33c5-106">管理対象デバイスの概要データ</span><span class="sxs-lookup"><span data-stu-id="a33c5-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="a33c5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a33c5-107">Methods</span></span>
|<span data-ttu-id="a33c5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a33c5-108">Method</span></span>|<span data-ttu-id="a33c5-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a33c5-109">Return Type</span></span>|<span data-ttu-id="a33c5-110">説明</span><span class="sxs-lookup"><span data-stu-id="a33c5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a33c5-111">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a33c5-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="a33c5-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a33c5-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="a33c5-113">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a33c5-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="a33c5-114">managedDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="a33c5-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="a33c5-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a33c5-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="a33c5-116">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a33c5-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a33c5-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a33c5-117">Properties</span></span>
|<span data-ttu-id="a33c5-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a33c5-118">Property</span></span>|<span data-ttu-id="a33c5-119">型</span><span class="sxs-lookup"><span data-stu-id="a33c5-119">Type</span></span>|<span data-ttu-id="a33c5-120">説明</span><span class="sxs-lookup"><span data-stu-id="a33c5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a33c5-121">id</span><span class="sxs-lookup"><span data-stu-id="a33c5-121">id</span></span>|<span data-ttu-id="a33c5-122">String</span><span class="sxs-lookup"><span data-stu-id="a33c5-122">String</span></span>|<span data-ttu-id="a33c5-123">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="a33c5-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="a33c5-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a33c5-124">enrolledDeviceCount</span></span>|<span data-ttu-id="a33c5-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a33c5-125">Int32</span></span>|<span data-ttu-id="a33c5-126">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="a33c5-126">Total enrolled device count.</span></span> <span data-ttu-id="a33c5-127">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="a33c5-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="a33c5-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="a33c5-128">mdmEnrolledCount</span></span>|<span data-ttu-id="a33c5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="a33c5-129">Int32</span></span>|<span data-ttu-id="a33c5-130">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a33c5-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="a33c5-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a33c5-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="a33c5-132">Int32</span><span class="sxs-lookup"><span data-stu-id="a33c5-132">Int32</span></span>|<span data-ttu-id="a33c5-133">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="a33c5-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="a33c5-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a33c5-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="a33c5-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a33c5-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="a33c5-136">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="a33c5-136">Device operating system summary.</span></span>|
|<span data-ttu-id="a33c5-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="a33c5-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="a33c5-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="a33c5-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="a33c5-139">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="a33c5-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="a33c5-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="a33c5-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="a33c5-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="a33c5-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="a33c5-142">アカウントの管理対象デバイスのモデルと製造 meatadata</span><span class="sxs-lookup"><span data-stu-id="a33c5-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="a33c5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a33c5-143">lastModifiedDateTime</span></span>|<span data-ttu-id="a33c5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a33c5-144">DateTimeOffset</span></span>|<span data-ttu-id="a33c5-145">デバイスの最終変更日時の概要</span><span class="sxs-lookup"><span data-stu-id="a33c5-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="a33c5-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a33c5-146">Relationships</span></span>
<span data-ttu-id="a33c5-147">なし</span><span class="sxs-lookup"><span data-stu-id="a33c5-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a33c5-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a33c5-148">JSON Representation</span></span>
<span data-ttu-id="a33c5-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a33c5-149">Here is a JSON representation of the resource.</span></span>
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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "String"
    ],
    "deviceManufacturers": [
      "String"
    ]
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```





