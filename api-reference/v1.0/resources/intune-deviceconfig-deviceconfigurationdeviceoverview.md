---
title: deviceConfigurationDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 50ed64b516f94d0e5e9eca07440d8360e8a19708
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845725"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="d98bc-103">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d98bc-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="d98bc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d98bc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d98bc-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d98bc-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="d98bc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d98bc-106">Methods</span></span>
|<span data-ttu-id="d98bc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d98bc-107">Method</span></span>|<span data-ttu-id="d98bc-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d98bc-108">Return Type</span></span>|<span data-ttu-id="d98bc-109">説明</span><span class="sxs-lookup"><span data-stu-id="d98bc-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d98bc-110">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d98bc-110">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="d98bc-111">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d98bc-111">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="d98bc-112">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d98bc-112">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="d98bc-113">Update deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d98bc-113">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="d98bc-114">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d98bc-114">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="d98bc-115">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d98bc-115">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d98bc-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d98bc-116">Properties</span></span>
|<span data-ttu-id="d98bc-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d98bc-117">Property</span></span>|<span data-ttu-id="d98bc-118">種類</span><span class="sxs-lookup"><span data-stu-id="d98bc-118">Type</span></span>|<span data-ttu-id="d98bc-119">説明</span><span class="sxs-lookup"><span data-stu-id="d98bc-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98bc-120">ID</span><span class="sxs-lookup"><span data-stu-id="d98bc-120">id</span></span>|<span data-ttu-id="d98bc-121">String</span><span class="sxs-lookup"><span data-stu-id="d98bc-121">String</span></span>|<span data-ttu-id="d98bc-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d98bc-122">Key of the entity.</span></span>|
|<span data-ttu-id="d98bc-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d98bc-123">pendingCount</span></span>|<span data-ttu-id="d98bc-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d98bc-124">Int32</span></span>|<span data-ttu-id="d98bc-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d98bc-125">Number of pending devices</span></span>|
|<span data-ttu-id="d98bc-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d98bc-126">notApplicableCount</span></span>|<span data-ttu-id="d98bc-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d98bc-127">Int32</span></span>|<span data-ttu-id="d98bc-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d98bc-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="d98bc-129">successCount</span><span class="sxs-lookup"><span data-stu-id="d98bc-129">successCount</span></span>|<span data-ttu-id="d98bc-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d98bc-130">Int32</span></span>|<span data-ttu-id="d98bc-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d98bc-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="d98bc-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="d98bc-132">errorCount</span></span>|<span data-ttu-id="d98bc-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d98bc-133">Int32</span></span>|<span data-ttu-id="d98bc-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d98bc-134">Number of error devices</span></span>|
|<span data-ttu-id="d98bc-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="d98bc-135">failedCount</span></span>|<span data-ttu-id="d98bc-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d98bc-136">Int32</span></span>|<span data-ttu-id="d98bc-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d98bc-137">Number of failed devices</span></span>|
|<span data-ttu-id="d98bc-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d98bc-138">lastUpdateDateTime</span></span>|<span data-ttu-id="d98bc-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d98bc-139">DateTimeOffset</span></span>|<span data-ttu-id="d98bc-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="d98bc-140">Last update time</span></span>|
|<span data-ttu-id="d98bc-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d98bc-141">configurationVersion</span></span>|<span data-ttu-id="d98bc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d98bc-142">Int32</span></span>|<span data-ttu-id="d98bc-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="d98bc-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="d98bc-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d98bc-144">Relationships</span></span>
<span data-ttu-id="d98bc-145">なし</span><span class="sxs-lookup"><span data-stu-id="d98bc-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d98bc-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d98bc-146">JSON Representation</span></span>
<span data-ttu-id="d98bc-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d98bc-147">Here is a JSON representation of the resource.</span></span>
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



