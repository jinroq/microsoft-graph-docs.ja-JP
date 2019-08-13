---
title: deviceManagementIntentDeviceSettingStateSummary リソースの種類
description: 目的に対するデバイス設定状態の概要を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b162728601d40fef304522af583d4cae6fc62d68
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371755"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a><span data-ttu-id="c74c7-103">deviceManagementIntentDeviceSettingStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c74c7-103">deviceManagementIntentDeviceSettingStateSummary resource type</span></span>

> <span data-ttu-id="c74c7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c74c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c74c7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c74c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c74c7-106">目的に対するデバイス設定状態の概要を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="c74c7-106">Entity that represents device setting state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="c74c7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c74c7-107">Methods</span></span>
|<span data-ttu-id="c74c7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c74c7-108">Method</span></span>|<span data-ttu-id="c74c7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c74c7-109">Return Type</span></span>|<span data-ttu-id="c74c7-110">説明</span><span class="sxs-lookup"><span data-stu-id="c74c7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c74c7-111">リスト deviceManagementIntentDeviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c74c7-111">List deviceManagementIntentDeviceSettingStateSummaries</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-list.md)|<span data-ttu-id="c74c7-112">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c74c7-112">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) collection</span></span>|<span data-ttu-id="c74c7-113">[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c74c7-113">List properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="c74c7-114">DeviceManagementIntentDeviceSettingStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="c74c7-114">Get deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-get.md)|[<span data-ttu-id="c74c7-115">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="c74c7-115">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="c74c7-116">[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c74c7-116">Read properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="c74c7-117">DeviceManagementIntentDeviceSettingStateSummary を作成する</span><span class="sxs-lookup"><span data-stu-id="c74c7-117">Create deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-create.md)|[<span data-ttu-id="c74c7-118">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="c74c7-118">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="c74c7-119">新しい[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c74c7-119">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="c74c7-120">DeviceManagementIntentDeviceSettingStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="c74c7-120">Delete deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-delete.md)|<span data-ttu-id="c74c7-121">None</span><span class="sxs-lookup"><span data-stu-id="c74c7-121">None</span></span>|<span data-ttu-id="c74c7-122">[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c74c7-122">Deletes a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>|
|[<span data-ttu-id="c74c7-123">DeviceManagementIntentDeviceSettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="c74c7-123">Update deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-update.md)|[<span data-ttu-id="c74c7-124">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="c74c7-124">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="c74c7-125">[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c74c7-125">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c74c7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c74c7-126">Properties</span></span>
|<span data-ttu-id="c74c7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c74c7-127">Property</span></span>|<span data-ttu-id="c74c7-128">型</span><span class="sxs-lookup"><span data-stu-id="c74c7-128">Type</span></span>|<span data-ttu-id="c74c7-129">説明</span><span class="sxs-lookup"><span data-stu-id="c74c7-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c74c7-130">id</span><span class="sxs-lookup"><span data-stu-id="c74c7-130">id</span></span>|<span data-ttu-id="c74c7-131">String</span><span class="sxs-lookup"><span data-stu-id="c74c7-131">String</span></span>|<span data-ttu-id="c74c7-132">ID</span><span class="sxs-lookup"><span data-stu-id="c74c7-132">The ID</span></span>|
|<span data-ttu-id="c74c7-133">settingName</span><span class="sxs-lookup"><span data-stu-id="c74c7-133">settingName</span></span>|<span data-ttu-id="c74c7-134">String</span><span class="sxs-lookup"><span data-stu-id="c74c7-134">String</span></span>|<span data-ttu-id="c74c7-135">設定の名前</span><span class="sxs-lookup"><span data-stu-id="c74c7-135">Name of a setting</span></span>|
|<span data-ttu-id="c74c7-136">compliantCount</span><span class="sxs-lookup"><span data-stu-id="c74c7-136">compliantCount</span></span>|<span data-ttu-id="c74c7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c74c7-137">Int32</span></span>|<span data-ttu-id="c74c7-138">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="c74c7-138">Number of compliant devices</span></span>|
|<span data-ttu-id="c74c7-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c74c7-139">conflictCount</span></span>|<span data-ttu-id="c74c7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c74c7-140">Int32</span></span>|<span data-ttu-id="c74c7-141">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c74c7-141">Number of devices in conflict</span></span>|
|<span data-ttu-id="c74c7-142">errorCount</span><span class="sxs-lookup"><span data-stu-id="c74c7-142">errorCount</span></span>|<span data-ttu-id="c74c7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c74c7-143">Int32</span></span>|<span data-ttu-id="c74c7-144">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="c74c7-144">Number of error devices</span></span>|
|<span data-ttu-id="c74c7-145">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="c74c7-145">nonCompliantCount</span></span>|<span data-ttu-id="c74c7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c74c7-146">Int32</span></span>|<span data-ttu-id="c74c7-147">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c74c7-147">Number of non compliant devices</span></span>|
|<span data-ttu-id="c74c7-148">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c74c7-148">notApplicableCount</span></span>|<span data-ttu-id="c74c7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c74c7-149">Int32</span></span>|<span data-ttu-id="c74c7-150">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c74c7-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="c74c7-151">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="c74c7-151">remediatedCount</span></span>|<span data-ttu-id="c74c7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c74c7-152">Int32</span></span>|<span data-ttu-id="c74c7-153">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c74c7-153">Number of remediated devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c74c7-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c74c7-154">Relationships</span></span>
<span data-ttu-id="c74c7-155">なし</span><span class="sxs-lookup"><span data-stu-id="c74c7-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c74c7-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c74c7-156">JSON Representation</span></span>
<span data-ttu-id="c74c7-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c74c7-157">Here is a JSON representation of the resource.</span></span>
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



