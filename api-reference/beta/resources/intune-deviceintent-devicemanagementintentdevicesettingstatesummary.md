---
title: deviceManagementIntentDeviceSettingStateSummary リソースの種類
description: 目的に対するデバイス設定状態の概要を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20eb5e9ae2941d1762a7cad634c9e6f5b3f2c24e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943425"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a><span data-ttu-id="3f901-103">deviceManagementIntentDeviceSettingStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3f901-103">deviceManagementIntentDeviceSettingStateSummary resource type</span></span>

> <span data-ttu-id="3f901-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f901-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f901-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f901-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f901-106">目的に対するデバイス設定状態の概要を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="3f901-106">Entity that represents device setting state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="3f901-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f901-107">Methods</span></span>
|<span data-ttu-id="3f901-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f901-108">Method</span></span>|<span data-ttu-id="3f901-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3f901-109">Return Type</span></span>|<span data-ttu-id="3f901-110">説明</span><span class="sxs-lookup"><span data-stu-id="3f901-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f901-111">リスト deviceManagementIntentDeviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3f901-111">List deviceManagementIntentDeviceSettingStateSummaries</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-list.md)|<span data-ttu-id="3f901-112">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3f901-112">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) collection</span></span>|<span data-ttu-id="3f901-113">[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3f901-113">List properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="3f901-114">DeviceManagementIntentDeviceSettingStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="3f901-114">Get deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-get.md)|[<span data-ttu-id="3f901-115">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="3f901-115">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="3f901-116">[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3f901-116">Read properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="3f901-117">DeviceManagementIntentDeviceSettingStateSummary を作成する</span><span class="sxs-lookup"><span data-stu-id="3f901-117">Create deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-create.md)|[<span data-ttu-id="3f901-118">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="3f901-118">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="3f901-119">新しい[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3f901-119">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="3f901-120">DeviceManagementIntentDeviceSettingStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="3f901-120">Delete deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-delete.md)|<span data-ttu-id="3f901-121">None</span><span class="sxs-lookup"><span data-stu-id="3f901-121">None</span></span>|<span data-ttu-id="3f901-122">[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="3f901-122">Deletes a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>|
|[<span data-ttu-id="3f901-123">DeviceManagementIntentDeviceSettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="3f901-123">Update deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-update.md)|[<span data-ttu-id="3f901-124">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="3f901-124">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="3f901-125">[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3f901-125">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f901-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f901-126">Properties</span></span>
|<span data-ttu-id="3f901-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f901-127">Property</span></span>|<span data-ttu-id="3f901-128">型</span><span class="sxs-lookup"><span data-stu-id="3f901-128">Type</span></span>|<span data-ttu-id="3f901-129">説明</span><span class="sxs-lookup"><span data-stu-id="3f901-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f901-130">id</span><span class="sxs-lookup"><span data-stu-id="3f901-130">id</span></span>|<span data-ttu-id="3f901-131">String</span><span class="sxs-lookup"><span data-stu-id="3f901-131">String</span></span>|<span data-ttu-id="3f901-132">ID</span><span class="sxs-lookup"><span data-stu-id="3f901-132">The ID</span></span>|
|<span data-ttu-id="3f901-133">settingName</span><span class="sxs-lookup"><span data-stu-id="3f901-133">settingName</span></span>|<span data-ttu-id="3f901-134">String</span><span class="sxs-lookup"><span data-stu-id="3f901-134">String</span></span>|<span data-ttu-id="3f901-135">設定の名前</span><span class="sxs-lookup"><span data-stu-id="3f901-135">Name of a setting</span></span>|
|<span data-ttu-id="3f901-136">compliantCount</span><span class="sxs-lookup"><span data-stu-id="3f901-136">compliantCount</span></span>|<span data-ttu-id="3f901-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3f901-137">Int32</span></span>|<span data-ttu-id="3f901-138">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="3f901-138">Number of compliant devices</span></span>|
|<span data-ttu-id="3f901-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="3f901-139">conflictCount</span></span>|<span data-ttu-id="3f901-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3f901-140">Int32</span></span>|<span data-ttu-id="3f901-141">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3f901-141">Number of devices in conflict</span></span>|
|<span data-ttu-id="3f901-142">errorCount</span><span class="sxs-lookup"><span data-stu-id="3f901-142">errorCount</span></span>|<span data-ttu-id="3f901-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3f901-143">Int32</span></span>|<span data-ttu-id="3f901-144">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="3f901-144">Number of error devices</span></span>|
|<span data-ttu-id="3f901-145">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="3f901-145">nonCompliantCount</span></span>|<span data-ttu-id="3f901-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3f901-146">Int32</span></span>|<span data-ttu-id="3f901-147">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3f901-147">Number of non compliant devices</span></span>|
|<span data-ttu-id="3f901-148">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="3f901-148">notApplicableCount</span></span>|<span data-ttu-id="3f901-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3f901-149">Int32</span></span>|<span data-ttu-id="3f901-150">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3f901-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="3f901-151">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="3f901-151">remediatedCount</span></span>|<span data-ttu-id="3f901-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3f901-152">Int32</span></span>|<span data-ttu-id="3f901-153">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3f901-153">Number of remediated devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f901-154">関係</span><span class="sxs-lookup"><span data-stu-id="3f901-154">Relationships</span></span>
<span data-ttu-id="3f901-155">なし</span><span class="sxs-lookup"><span data-stu-id="3f901-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f901-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3f901-156">JSON Representation</span></span>
<span data-ttu-id="3f901-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3f901-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceSettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "compliantCount": 1024,
  "conflictCount": 1024,
  "errorCount": 1024,
  "nonCompliantCount": 1024,
  "notApplicableCount": 1024,
  "remediatedCount": 1024
}
```




