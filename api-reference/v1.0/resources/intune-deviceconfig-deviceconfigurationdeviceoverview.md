---
title: deviceConfigurationDeviceOverview リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 068292de3f8f128e9052cada73ab1e00107741b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021797"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="dd757-103">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dd757-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="dd757-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd757-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd757-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dd757-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="dd757-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="dd757-106">Methods</span></span>
|<span data-ttu-id="dd757-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dd757-107">Method</span></span>|<span data-ttu-id="dd757-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dd757-108">Return Type</span></span>|<span data-ttu-id="dd757-109">説明</span><span class="sxs-lookup"><span data-stu-id="dd757-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dd757-110">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="dd757-110">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="dd757-111">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="dd757-111">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="dd757-112">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dd757-112">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="dd757-113">Update deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="dd757-113">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="dd757-114">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="dd757-114">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="dd757-115">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dd757-115">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd757-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd757-116">Properties</span></span>
|<span data-ttu-id="dd757-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd757-117">Property</span></span>|<span data-ttu-id="dd757-118">型</span><span class="sxs-lookup"><span data-stu-id="dd757-118">Type</span></span>|<span data-ttu-id="dd757-119">説明</span><span class="sxs-lookup"><span data-stu-id="dd757-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd757-120">id</span><span class="sxs-lookup"><span data-stu-id="dd757-120">id</span></span>|<span data-ttu-id="dd757-121">String</span><span class="sxs-lookup"><span data-stu-id="dd757-121">String</span></span>|<span data-ttu-id="dd757-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dd757-122">Key of the entity.</span></span>|
|<span data-ttu-id="dd757-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="dd757-123">pendingCount</span></span>|<span data-ttu-id="dd757-124">Int32</span><span class="sxs-lookup"><span data-stu-id="dd757-124">Int32</span></span>|<span data-ttu-id="dd757-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="dd757-125">Number of pending devices</span></span>|
|<span data-ttu-id="dd757-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="dd757-126">notApplicableCount</span></span>|<span data-ttu-id="dd757-127">Int32</span><span class="sxs-lookup"><span data-stu-id="dd757-127">Int32</span></span>|<span data-ttu-id="dd757-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="dd757-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="dd757-129">successCount</span><span class="sxs-lookup"><span data-stu-id="dd757-129">successCount</span></span>|<span data-ttu-id="dd757-130">Int32</span><span class="sxs-lookup"><span data-stu-id="dd757-130">Int32</span></span>|<span data-ttu-id="dd757-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="dd757-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="dd757-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="dd757-132">errorCount</span></span>|<span data-ttu-id="dd757-133">Int32</span><span class="sxs-lookup"><span data-stu-id="dd757-133">Int32</span></span>|<span data-ttu-id="dd757-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="dd757-134">Number of error devices</span></span>|
|<span data-ttu-id="dd757-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="dd757-135">failedCount</span></span>|<span data-ttu-id="dd757-136">Int32</span><span class="sxs-lookup"><span data-stu-id="dd757-136">Int32</span></span>|<span data-ttu-id="dd757-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="dd757-137">Number of failed devices</span></span>|
|<span data-ttu-id="dd757-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="dd757-138">lastUpdateDateTime</span></span>|<span data-ttu-id="dd757-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd757-139">DateTimeOffset</span></span>|<span data-ttu-id="dd757-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="dd757-140">Last update time</span></span>|
|<span data-ttu-id="dd757-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="dd757-141">configurationVersion</span></span>|<span data-ttu-id="dd757-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dd757-142">Int32</span></span>|<span data-ttu-id="dd757-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="dd757-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd757-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dd757-144">Relationships</span></span>
<span data-ttu-id="dd757-145">なし</span><span class="sxs-lookup"><span data-stu-id="dd757-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dd757-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd757-146">JSON Representation</span></span>
<span data-ttu-id="dd757-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dd757-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
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



