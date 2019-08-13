---
title: deviceManagementScriptRunSummary リソースの種類
description: デバイス管理スクリプトの実行の概要のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9d2b0b92287a045607c02e271155e2e74a2fa90
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370026"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="0cb9d-103">deviceManagementScriptRunSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cb9d-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="0cb9d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cb9d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cb9d-106">デバイス管理スクリプトの実行の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="0cb9d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cb9d-107">Methods</span></span>
|<span data-ttu-id="0cb9d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cb9d-108">Method</span></span>|<span data-ttu-id="0cb9d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0cb9d-109">Return Type</span></span>|<span data-ttu-id="0cb9d-110">説明</span><span class="sxs-lookup"><span data-stu-id="0cb9d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0cb9d-111">DeviceManagementScriptRunSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="0cb9d-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="0cb9d-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="0cb9d-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="0cb9d-113">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="0cb9d-114">DeviceManagementScriptRunSummary の更新</span><span class="sxs-lookup"><span data-stu-id="0cb9d-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="0cb9d-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="0cb9d-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="0cb9d-116">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cb9d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cb9d-117">Properties</span></span>
|<span data-ttu-id="0cb9d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cb9d-118">Property</span></span>|<span data-ttu-id="0cb9d-119">型</span><span class="sxs-lookup"><span data-stu-id="0cb9d-119">Type</span></span>|<span data-ttu-id="0cb9d-120">説明</span><span class="sxs-lookup"><span data-stu-id="0cb9d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cb9d-121">id</span><span class="sxs-lookup"><span data-stu-id="0cb9d-121">id</span></span>|<span data-ttu-id="0cb9d-122">String</span><span class="sxs-lookup"><span data-stu-id="0cb9d-122">String</span></span>|<span data-ttu-id="0cb9d-123">デバイス管理スクリプト実行の概要エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="0cb9d-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cb9d-124">successDeviceCount</span></span>|<span data-ttu-id="0cb9d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0cb9d-125">Int32</span></span>|<span data-ttu-id="0cb9d-126">成功したデバイス数。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-126">Success device count.</span></span>|
|<span data-ttu-id="0cb9d-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cb9d-127">errorDeviceCount</span></span>|<span data-ttu-id="0cb9d-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0cb9d-128">Int32</span></span>|<span data-ttu-id="0cb9d-129">エラーデバイス数。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-129">Error device count.</span></span>|
|<span data-ttu-id="0cb9d-130">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cb9d-130">compliantDeviceCount</span></span>|<span data-ttu-id="0cb9d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0cb9d-131">Int32</span></span>|<span data-ttu-id="0cb9d-132">準拠しているデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-132">Compliant device count.</span></span>|
|<span data-ttu-id="0cb9d-133">notCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cb9d-133">notCompliantDeviceCount</span></span>|<span data-ttu-id="0cb9d-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0cb9d-134">Int32</span></span>|<span data-ttu-id="0cb9d-135">準拠していないデバイス数。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-135">Not Compliant device count.</span></span>|
|<span data-ttu-id="0cb9d-136">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cb9d-136">pendingDeviceCount</span></span>|<span data-ttu-id="0cb9d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0cb9d-137">Int32</span></span>|<span data-ttu-id="0cb9d-138">保留中のデバイス数。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-138">Pending device count.</span></span>|
|<span data-ttu-id="0cb9d-139">successUserCount</span><span class="sxs-lookup"><span data-stu-id="0cb9d-139">successUserCount</span></span>|<span data-ttu-id="0cb9d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0cb9d-140">Int32</span></span>|<span data-ttu-id="0cb9d-141">成功したユーザー数。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-141">Success user count.</span></span>|
|<span data-ttu-id="0cb9d-142">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="0cb9d-142">errorUserCount</span></span>|<span data-ttu-id="0cb9d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0cb9d-143">Int32</span></span>|<span data-ttu-id="0cb9d-144">エラーユーザー数。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-144">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cb9d-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0cb9d-145">Relationships</span></span>
<span data-ttu-id="0cb9d-146">なし</span><span class="sxs-lookup"><span data-stu-id="0cb9d-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cb9d-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cb9d-147">JSON Representation</span></span>
<span data-ttu-id="0cb9d-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0cb9d-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "notCompliantDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```



