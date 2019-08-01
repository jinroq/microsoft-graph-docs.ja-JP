---
title: deviceConfigurationDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25abfce9ad69ea6f658a8883cb227806362a6cff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028442"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="68852-103">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68852-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="68852-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68852-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68852-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="68852-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="68852-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="68852-106">Methods</span></span>
|<span data-ttu-id="68852-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="68852-107">Method</span></span>|<span data-ttu-id="68852-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="68852-108">Return Type</span></span>|<span data-ttu-id="68852-109">説明</span><span class="sxs-lookup"><span data-stu-id="68852-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68852-110">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="68852-110">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="68852-111">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="68852-111">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="68852-112">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="68852-112">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="68852-113">Update deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="68852-113">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="68852-114">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="68852-114">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="68852-115">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="68852-115">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="68852-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68852-116">Properties</span></span>
|<span data-ttu-id="68852-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68852-117">Property</span></span>|<span data-ttu-id="68852-118">型</span><span class="sxs-lookup"><span data-stu-id="68852-118">Type</span></span>|<span data-ttu-id="68852-119">説明</span><span class="sxs-lookup"><span data-stu-id="68852-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68852-120">id</span><span class="sxs-lookup"><span data-stu-id="68852-120">id</span></span>|<span data-ttu-id="68852-121">String</span><span class="sxs-lookup"><span data-stu-id="68852-121">String</span></span>|<span data-ttu-id="68852-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="68852-122">Key of the entity.</span></span>|
|<span data-ttu-id="68852-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="68852-123">pendingCount</span></span>|<span data-ttu-id="68852-124">Int32</span><span class="sxs-lookup"><span data-stu-id="68852-124">Int32</span></span>|<span data-ttu-id="68852-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="68852-125">Number of pending devices</span></span>|
|<span data-ttu-id="68852-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="68852-126">notApplicableCount</span></span>|<span data-ttu-id="68852-127">Int32</span><span class="sxs-lookup"><span data-stu-id="68852-127">Int32</span></span>|<span data-ttu-id="68852-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="68852-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="68852-129">successCount</span><span class="sxs-lookup"><span data-stu-id="68852-129">successCount</span></span>|<span data-ttu-id="68852-130">Int32</span><span class="sxs-lookup"><span data-stu-id="68852-130">Int32</span></span>|<span data-ttu-id="68852-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="68852-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="68852-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="68852-132">errorCount</span></span>|<span data-ttu-id="68852-133">Int32</span><span class="sxs-lookup"><span data-stu-id="68852-133">Int32</span></span>|<span data-ttu-id="68852-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="68852-134">Number of error devices</span></span>|
|<span data-ttu-id="68852-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="68852-135">failedCount</span></span>|<span data-ttu-id="68852-136">Int32</span><span class="sxs-lookup"><span data-stu-id="68852-136">Int32</span></span>|<span data-ttu-id="68852-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="68852-137">Number of failed devices</span></span>|
|<span data-ttu-id="68852-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="68852-138">lastUpdateDateTime</span></span>|<span data-ttu-id="68852-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68852-139">DateTimeOffset</span></span>|<span data-ttu-id="68852-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="68852-140">Last update time</span></span>|
|<span data-ttu-id="68852-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="68852-141">configurationVersion</span></span>|<span data-ttu-id="68852-142">Int32</span><span class="sxs-lookup"><span data-stu-id="68852-142">Int32</span></span>|<span data-ttu-id="68852-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="68852-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="68852-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68852-144">Relationships</span></span>
<span data-ttu-id="68852-145">なし</span><span class="sxs-lookup"><span data-stu-id="68852-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68852-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68852-146">JSON Representation</span></span>
<span data-ttu-id="68852-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68852-147">Here is a JSON representation of the resource.</span></span>
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



