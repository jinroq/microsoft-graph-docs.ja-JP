---
title: deviceConfigurationDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe9c94c5ca430f72e2433755533ccb221063cda7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573397"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="b0ef6-103">deviceConfigurationDeviceOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0ef6-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="b0ef6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0ef6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0ef6-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b0ef6-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="b0ef6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0ef6-106">Methods</span></span>
|<span data-ttu-id="b0ef6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0ef6-107">Method</span></span>|<span data-ttu-id="b0ef6-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b0ef6-108">Return Type</span></span>|<span data-ttu-id="b0ef6-109">説明</span><span class="sxs-lookup"><span data-stu-id="b0ef6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0ef6-110">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b0ef6-110">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="b0ef6-111">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b0ef6-111">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="b0ef6-112">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b0ef6-112">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="b0ef6-113">Update deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b0ef6-113">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="b0ef6-114">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b0ef6-114">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="b0ef6-115">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b0ef6-115">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0ef6-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0ef6-116">Properties</span></span>
|<span data-ttu-id="b0ef6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0ef6-117">Property</span></span>|<span data-ttu-id="b0ef6-118">型</span><span class="sxs-lookup"><span data-stu-id="b0ef6-118">Type</span></span>|<span data-ttu-id="b0ef6-119">説明</span><span class="sxs-lookup"><span data-stu-id="b0ef6-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0ef6-120">id</span><span class="sxs-lookup"><span data-stu-id="b0ef6-120">id</span></span>|<span data-ttu-id="b0ef6-121">String</span><span class="sxs-lookup"><span data-stu-id="b0ef6-121">String</span></span>|<span data-ttu-id="b0ef6-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b0ef6-122">Key of the entity.</span></span>|
|<span data-ttu-id="b0ef6-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b0ef6-123">pendingCount</span></span>|<span data-ttu-id="b0ef6-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ef6-124">Int32</span></span>|<span data-ttu-id="b0ef6-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ef6-125">Number of pending devices</span></span>|
|<span data-ttu-id="b0ef6-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b0ef6-126">notApplicableCount</span></span>|<span data-ttu-id="b0ef6-127">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ef6-127">Int32</span></span>|<span data-ttu-id="b0ef6-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ef6-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="b0ef6-129">successCount</span><span class="sxs-lookup"><span data-stu-id="b0ef6-129">successCount</span></span>|<span data-ttu-id="b0ef6-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ef6-130">Int32</span></span>|<span data-ttu-id="b0ef6-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ef6-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="b0ef6-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="b0ef6-132">errorCount</span></span>|<span data-ttu-id="b0ef6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ef6-133">Int32</span></span>|<span data-ttu-id="b0ef6-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ef6-134">Number of error devices</span></span>|
|<span data-ttu-id="b0ef6-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="b0ef6-135">failedCount</span></span>|<span data-ttu-id="b0ef6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ef6-136">Int32</span></span>|<span data-ttu-id="b0ef6-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b0ef6-137">Number of failed devices</span></span>|
|<span data-ttu-id="b0ef6-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b0ef6-138">lastUpdateDateTime</span></span>|<span data-ttu-id="b0ef6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0ef6-139">DateTimeOffset</span></span>|<span data-ttu-id="b0ef6-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="b0ef6-140">Last update time</span></span>|
|<span data-ttu-id="b0ef6-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b0ef6-141">configurationVersion</span></span>|<span data-ttu-id="b0ef6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ef6-142">Int32</span></span>|<span data-ttu-id="b0ef6-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="b0ef6-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0ef6-144">関係</span><span class="sxs-lookup"><span data-stu-id="b0ef6-144">Relationships</span></span>
<span data-ttu-id="b0ef6-145">なし</span><span class="sxs-lookup"><span data-stu-id="b0ef6-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0ef6-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0ef6-146">JSON Representation</span></span>
<span data-ttu-id="b0ef6-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0ef6-147">Here is a JSON representation of the resource.</span></span>
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



