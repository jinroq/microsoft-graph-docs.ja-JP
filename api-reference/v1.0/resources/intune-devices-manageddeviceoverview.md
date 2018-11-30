---
title: managedDeviceOverview リソースの種類
description: 管理対象デバイスの概要データ
ms.openlocfilehash: 0d99d16b8f6ca8f71e419f39f473571d80703dc1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022825"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="3086c-103">managedDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3086c-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="3086c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3086c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3086c-105">管理対象デバイスの概要データ</span><span class="sxs-lookup"><span data-stu-id="3086c-105">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="3086c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3086c-106">Methods</span></span>
|<span data-ttu-id="3086c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3086c-107">Method</span></span>|<span data-ttu-id="3086c-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3086c-108">Return Type</span></span>|<span data-ttu-id="3086c-109">説明</span><span class="sxs-lookup"><span data-stu-id="3086c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3086c-110">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3086c-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="3086c-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3086c-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="3086c-112">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3086c-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="3086c-113">Update managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3086c-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="3086c-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3086c-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="3086c-115">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3086c-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3086c-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3086c-116">Properties</span></span>
|<span data-ttu-id="3086c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3086c-117">Property</span></span>|<span data-ttu-id="3086c-118">型</span><span class="sxs-lookup"><span data-stu-id="3086c-118">Type</span></span>|<span data-ttu-id="3086c-119">説明</span><span class="sxs-lookup"><span data-stu-id="3086c-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3086c-120">id</span><span class="sxs-lookup"><span data-stu-id="3086c-120">id</span></span>|<span data-ttu-id="3086c-121">String</span><span class="sxs-lookup"><span data-stu-id="3086c-121">String</span></span>|<span data-ttu-id="3086c-122">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="3086c-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="3086c-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3086c-123">enrolledDeviceCount</span></span>|<span data-ttu-id="3086c-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3086c-124">Int32</span></span>|<span data-ttu-id="3086c-125">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="3086c-125">Total enrolled device count.</span></span> <span data-ttu-id="3086c-126">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="3086c-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="3086c-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="3086c-127">mdmEnrolledCount</span></span>|<span data-ttu-id="3086c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3086c-128">Int32</span></span>|<span data-ttu-id="3086c-129">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3086c-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="3086c-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3086c-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="3086c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="3086c-131">Int32</span></span>|<span data-ttu-id="3086c-132">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3086c-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="3086c-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="3086c-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="3086c-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="3086c-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="3086c-135">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="3086c-135">Device operating system summary.</span></span>|
|<span data-ttu-id="3086c-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="3086c-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="3086c-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="3086c-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="3086c-138">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="3086c-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="3086c-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3086c-139">Relationships</span></span>
<span data-ttu-id="3086c-140">なし</span><span class="sxs-lookup"><span data-stu-id="3086c-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3086c-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3086c-141">JSON Representation</span></span>
<span data-ttu-id="3086c-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3086c-142">Here is a JSON representation of the resource.</span></span>
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



