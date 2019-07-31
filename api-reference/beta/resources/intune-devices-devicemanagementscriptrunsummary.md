---
title: deviceManagementScriptRunSummary リソースの種類
description: デバイス管理スクリプトの実行の概要のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a2486a52a5ce71805604f9e3d9b8d5bfdd6c85e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999837"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="54110-103">deviceManagementScriptRunSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54110-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="54110-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54110-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54110-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54110-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54110-106">デバイス管理スクリプトの実行の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54110-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="54110-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="54110-107">Methods</span></span>
|<span data-ttu-id="54110-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="54110-108">Method</span></span>|<span data-ttu-id="54110-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="54110-109">Return Type</span></span>|<span data-ttu-id="54110-110">説明</span><span class="sxs-lookup"><span data-stu-id="54110-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54110-111">DeviceManagementScriptRunSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="54110-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="54110-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="54110-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="54110-113">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="54110-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="54110-114">DeviceManagementScriptRunSummary の更新</span><span class="sxs-lookup"><span data-stu-id="54110-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="54110-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="54110-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="54110-116">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="54110-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="54110-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54110-117">Properties</span></span>
|<span data-ttu-id="54110-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54110-118">Property</span></span>|<span data-ttu-id="54110-119">型</span><span class="sxs-lookup"><span data-stu-id="54110-119">Type</span></span>|<span data-ttu-id="54110-120">説明</span><span class="sxs-lookup"><span data-stu-id="54110-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54110-121">id</span><span class="sxs-lookup"><span data-stu-id="54110-121">id</span></span>|<span data-ttu-id="54110-122">String</span><span class="sxs-lookup"><span data-stu-id="54110-122">String</span></span>|<span data-ttu-id="54110-123">デバイス管理スクリプト実行の概要エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="54110-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="54110-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54110-124">successDeviceCount</span></span>|<span data-ttu-id="54110-125">Int32</span><span class="sxs-lookup"><span data-stu-id="54110-125">Int32</span></span>|<span data-ttu-id="54110-126">成功したデバイス数。</span><span class="sxs-lookup"><span data-stu-id="54110-126">Success device count.</span></span>|
|<span data-ttu-id="54110-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54110-127">errorDeviceCount</span></span>|<span data-ttu-id="54110-128">Int32</span><span class="sxs-lookup"><span data-stu-id="54110-128">Int32</span></span>|<span data-ttu-id="54110-129">エラーデバイス数。</span><span class="sxs-lookup"><span data-stu-id="54110-129">Error device count.</span></span>|
|<span data-ttu-id="54110-130">successUserCount</span><span class="sxs-lookup"><span data-stu-id="54110-130">successUserCount</span></span>|<span data-ttu-id="54110-131">Int32</span><span class="sxs-lookup"><span data-stu-id="54110-131">Int32</span></span>|<span data-ttu-id="54110-132">成功したユーザー数。</span><span class="sxs-lookup"><span data-stu-id="54110-132">Success user count.</span></span>|
|<span data-ttu-id="54110-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="54110-133">errorUserCount</span></span>|<span data-ttu-id="54110-134">Int32</span><span class="sxs-lookup"><span data-stu-id="54110-134">Int32</span></span>|<span data-ttu-id="54110-135">エラーユーザー数。</span><span class="sxs-lookup"><span data-stu-id="54110-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54110-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54110-136">Relationships</span></span>
<span data-ttu-id="54110-137">なし</span><span class="sxs-lookup"><span data-stu-id="54110-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54110-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54110-138">JSON Representation</span></span>
<span data-ttu-id="54110-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54110-139">Here is a JSON representation of the resource.</span></span>
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
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```





