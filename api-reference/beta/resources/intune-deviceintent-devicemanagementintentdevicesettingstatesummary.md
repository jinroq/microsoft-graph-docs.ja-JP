---
title: deviceManagementIntentDeviceSettingStateSummary リソースの種類
description: 目的に対するデバイス設定状態の概要を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3c3e6a3630d3e28e62555db25565ab916dc7a91
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524058"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a><span data-ttu-id="b63a8-103">deviceManagementIntentDeviceSettingStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b63a8-103">deviceManagementIntentDeviceSettingStateSummary resource type</span></span>

> <span data-ttu-id="b63a8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b63a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b63a8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b63a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b63a8-106">目的に対するデバイス設定状態の概要を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="b63a8-106">Entity that represents device setting state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="b63a8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b63a8-107">Methods</span></span>
|<span data-ttu-id="b63a8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b63a8-108">Method</span></span>|<span data-ttu-id="b63a8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b63a8-109">Return Type</span></span>|<span data-ttu-id="b63a8-110">説明</span><span class="sxs-lookup"><span data-stu-id="b63a8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b63a8-111">リスト deviceManagementIntentDeviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="b63a8-111">List deviceManagementIntentDeviceSettingStateSummaries</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-list.md)|<span data-ttu-id="b63a8-112">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b63a8-112">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) collection</span></span>|<span data-ttu-id="b63a8-113">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b63a8-113">List properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="b63a8-114">deviceManagementIntentDeviceSettingStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="b63a8-114">Get deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-get.md)|[<span data-ttu-id="b63a8-115">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="b63a8-115">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="b63a8-116">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b63a8-116">Read properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="b63a8-117">deviceManagementIntentDeviceSettingStateSummary を作成する</span><span class="sxs-lookup"><span data-stu-id="b63a8-117">Create deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-create.md)|[<span data-ttu-id="b63a8-118">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="b63a8-118">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="b63a8-119">新しい[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b63a8-119">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|
|[<span data-ttu-id="b63a8-120">deviceManagementIntentDeviceSettingStateSummary の削除</span><span class="sxs-lookup"><span data-stu-id="b63a8-120">Delete deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-delete.md)|<span data-ttu-id="b63a8-121">なし</span><span class="sxs-lookup"><span data-stu-id="b63a8-121">None</span></span>|<span data-ttu-id="b63a8-122">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="b63a8-122">Deletes a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>|
|[<span data-ttu-id="b63a8-123">deviceManagementIntentDeviceSettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="b63a8-123">Update deviceManagementIntentDeviceSettingStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-update.md)|[<span data-ttu-id="b63a8-124">deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="b63a8-124">deviceManagementIntentDeviceSettingStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|<span data-ttu-id="b63a8-125">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b63a8-125">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b63a8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b63a8-126">Properties</span></span>
|<span data-ttu-id="b63a8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b63a8-127">Property</span></span>|<span data-ttu-id="b63a8-128">型</span><span class="sxs-lookup"><span data-stu-id="b63a8-128">Type</span></span>|<span data-ttu-id="b63a8-129">説明</span><span class="sxs-lookup"><span data-stu-id="b63a8-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b63a8-130">id</span><span class="sxs-lookup"><span data-stu-id="b63a8-130">id</span></span>|<span data-ttu-id="b63a8-131">String</span><span class="sxs-lookup"><span data-stu-id="b63a8-131">String</span></span>|<span data-ttu-id="b63a8-132">ID</span><span class="sxs-lookup"><span data-stu-id="b63a8-132">The ID</span></span>|
|<span data-ttu-id="b63a8-133">settingName</span><span class="sxs-lookup"><span data-stu-id="b63a8-133">settingName</span></span>|<span data-ttu-id="b63a8-134">String</span><span class="sxs-lookup"><span data-stu-id="b63a8-134">String</span></span>|<span data-ttu-id="b63a8-135">設定の名前</span><span class="sxs-lookup"><span data-stu-id="b63a8-135">Name of a setting</span></span>|
|<span data-ttu-id="b63a8-136">compliantCount</span><span class="sxs-lookup"><span data-stu-id="b63a8-136">compliantCount</span></span>|<span data-ttu-id="b63a8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b63a8-137">Int32</span></span>|<span data-ttu-id="b63a8-138">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="b63a8-138">Number of compliant devices</span></span>|
|<span data-ttu-id="b63a8-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b63a8-139">conflictCount</span></span>|<span data-ttu-id="b63a8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b63a8-140">Int32</span></span>|<span data-ttu-id="b63a8-141">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b63a8-141">Number of devices in conflict</span></span>|
|<span data-ttu-id="b63a8-142">errorCount</span><span class="sxs-lookup"><span data-stu-id="b63a8-142">errorCount</span></span>|<span data-ttu-id="b63a8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b63a8-143">Int32</span></span>|<span data-ttu-id="b63a8-144">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="b63a8-144">Number of error devices</span></span>|
|<span data-ttu-id="b63a8-145">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="b63a8-145">nonCompliantCount</span></span>|<span data-ttu-id="b63a8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b63a8-146">Int32</span></span>|<span data-ttu-id="b63a8-147">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b63a8-147">Number of non compliant devices</span></span>|
|<span data-ttu-id="b63a8-148">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b63a8-148">notApplicableCount</span></span>|<span data-ttu-id="b63a8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b63a8-149">Int32</span></span>|<span data-ttu-id="b63a8-150">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b63a8-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="b63a8-151">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="b63a8-151">remediatedCount</span></span>|<span data-ttu-id="b63a8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b63a8-152">Int32</span></span>|<span data-ttu-id="b63a8-153">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b63a8-153">Number of remediated devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b63a8-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b63a8-154">Relationships</span></span>
<span data-ttu-id="b63a8-155">なし</span><span class="sxs-lookup"><span data-stu-id="b63a8-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b63a8-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b63a8-156">JSON Representation</span></span>
<span data-ttu-id="b63a8-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b63a8-157">Here is a JSON representation of the resource.</span></span>
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







