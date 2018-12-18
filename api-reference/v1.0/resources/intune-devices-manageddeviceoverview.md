---
title: managedDeviceOverview リソースの種類
description: 管理対象デバイスの概要データ
author: tfitzmac
ms.openlocfilehash: c6c82338dfb696039d584f8a035a8e1427674fac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344073"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="7a80d-103">managedDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a80d-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="7a80d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a80d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a80d-105">管理対象デバイスの概要データ</span><span class="sxs-lookup"><span data-stu-id="7a80d-105">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="7a80d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a80d-106">Methods</span></span>
|<span data-ttu-id="7a80d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a80d-107">Method</span></span>|<span data-ttu-id="7a80d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7a80d-108">Return Type</span></span>|<span data-ttu-id="7a80d-109">説明</span><span class="sxs-lookup"><span data-stu-id="7a80d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a80d-110">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7a80d-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="7a80d-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7a80d-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="7a80d-112">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7a80d-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="7a80d-113">Update managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7a80d-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="7a80d-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7a80d-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="7a80d-115">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7a80d-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a80d-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a80d-116">Properties</span></span>
|<span data-ttu-id="7a80d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a80d-117">Property</span></span>|<span data-ttu-id="7a80d-118">種類</span><span class="sxs-lookup"><span data-stu-id="7a80d-118">Type</span></span>|<span data-ttu-id="7a80d-119">説明</span><span class="sxs-lookup"><span data-stu-id="7a80d-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a80d-120">ID</span><span class="sxs-lookup"><span data-stu-id="7a80d-120">id</span></span>|<span data-ttu-id="7a80d-121">String</span><span class="sxs-lookup"><span data-stu-id="7a80d-121">String</span></span>|<span data-ttu-id="7a80d-122">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="7a80d-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="7a80d-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a80d-123">enrolledDeviceCount</span></span>|<span data-ttu-id="7a80d-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7a80d-124">Int32</span></span>|<span data-ttu-id="7a80d-125">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="7a80d-125">Total enrolled device count.</span></span> <span data-ttu-id="7a80d-126">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="7a80d-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="7a80d-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="7a80d-127">mdmEnrolledCount</span></span>|<span data-ttu-id="7a80d-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7a80d-128">Int32</span></span>|<span data-ttu-id="7a80d-129">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="7a80d-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="7a80d-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a80d-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="7a80d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7a80d-131">Int32</span></span>|<span data-ttu-id="7a80d-132">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="7a80d-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="7a80d-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7a80d-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="7a80d-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7a80d-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="7a80d-135">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="7a80d-135">Device operating system summary.</span></span>|
|<span data-ttu-id="7a80d-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7a80d-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="7a80d-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7a80d-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="7a80d-138">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="7a80d-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a80d-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a80d-139">Relationships</span></span>
<span data-ttu-id="7a80d-140">なし</span><span class="sxs-lookup"><span data-stu-id="7a80d-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a80d-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a80d-141">JSON Representation</span></span>
<span data-ttu-id="7a80d-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a80d-142">Here is a JSON representation of the resource.</span></span>
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



