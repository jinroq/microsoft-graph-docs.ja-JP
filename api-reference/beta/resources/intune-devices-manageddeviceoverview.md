---
title: managedDeviceOverview リソースの種類
description: 管理対象デバイスの概要データ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 091871ed88903f4fcb3a3ad8be86e7b997f173b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932516"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="eb7f3-103">managedDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb7f3-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="eb7f3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eb7f3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb7f3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb7f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb7f3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eb7f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb7f3-107">管理対象デバイスの概要データ</span><span class="sxs-lookup"><span data-stu-id="eb7f3-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="eb7f3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="eb7f3-108">Methods</span></span>
|<span data-ttu-id="eb7f3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="eb7f3-109">Method</span></span>|<span data-ttu-id="eb7f3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="eb7f3-110">Return Type</span></span>|<span data-ttu-id="eb7f3-111">説明</span><span class="sxs-lookup"><span data-stu-id="eb7f3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eb7f3-112">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="eb7f3-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="eb7f3-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="eb7f3-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="eb7f3-114">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="eb7f3-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="eb7f3-115">Update managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="eb7f3-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="eb7f3-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="eb7f3-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="eb7f3-117">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="eb7f3-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb7f3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb7f3-118">Properties</span></span>
|<span data-ttu-id="eb7f3-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb7f3-119">Property</span></span>|<span data-ttu-id="eb7f3-120">種類</span><span class="sxs-lookup"><span data-stu-id="eb7f3-120">Type</span></span>|<span data-ttu-id="eb7f3-121">説明</span><span class="sxs-lookup"><span data-stu-id="eb7f3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb7f3-122">ID</span><span class="sxs-lookup"><span data-stu-id="eb7f3-122">id</span></span>|<span data-ttu-id="eb7f3-123">String</span><span class="sxs-lookup"><span data-stu-id="eb7f3-123">String</span></span>|<span data-ttu-id="eb7f3-124">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="eb7f3-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="eb7f3-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb7f3-125">enrolledDeviceCount</span></span>|<span data-ttu-id="eb7f3-126">Int32</span><span class="sxs-lookup"><span data-stu-id="eb7f3-126">Int32</span></span>|<span data-ttu-id="eb7f3-127">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="eb7f3-127">Total enrolled device count.</span></span> <span data-ttu-id="eb7f3-128">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="eb7f3-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="eb7f3-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="eb7f3-129">mdmEnrolledCount</span></span>|<span data-ttu-id="eb7f3-130">Int32</span><span class="sxs-lookup"><span data-stu-id="eb7f3-130">Int32</span></span>|<span data-ttu-id="eb7f3-131">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="eb7f3-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="eb7f3-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb7f3-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="eb7f3-133">Int32</span><span class="sxs-lookup"><span data-stu-id="eb7f3-133">Int32</span></span>|<span data-ttu-id="eb7f3-134">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="eb7f3-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="eb7f3-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="eb7f3-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="eb7f3-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="eb7f3-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="eb7f3-137">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="eb7f3-137">Device operating system summary.</span></span>|
|<span data-ttu-id="eb7f3-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="eb7f3-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="eb7f3-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="eb7f3-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="eb7f3-140">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="eb7f3-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="eb7f3-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="eb7f3-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="eb7f3-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="eb7f3-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="eb7f3-143">モデルと、アカウントで管理されているデバイスのメーカーの meatadata</span><span class="sxs-lookup"><span data-stu-id="eb7f3-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="eb7f3-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb7f3-144">lastModifiedDateTime</span></span>|<span data-ttu-id="eb7f3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb7f3-145">DateTimeOffset</span></span>|<span data-ttu-id="eb7f3-146">デバイスの概要の最後の更新日時</span><span class="sxs-lookup"><span data-stu-id="eb7f3-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb7f3-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eb7f3-147">Relationships</span></span>
<span data-ttu-id="eb7f3-148">なし</span><span class="sxs-lookup"><span data-stu-id="eb7f3-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb7f3-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb7f3-149">JSON Representation</span></span>
<span data-ttu-id="eb7f3-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb7f3-150">Here is a JSON representation of the resource.</span></span>
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





