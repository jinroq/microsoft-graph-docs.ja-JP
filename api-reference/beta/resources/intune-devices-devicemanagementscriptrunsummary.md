---
title: deviceManagementScriptRunSummary リソースの種類
description: デバイス管理スクリプトの実行の概要のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199b9efcdc3ea862502ea22d845480d990c99caf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995309"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="d9854-103">deviceManagementScriptRunSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9854-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="d9854-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9854-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9854-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9854-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9854-106">デバイス管理スクリプトの実行の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d9854-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="d9854-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d9854-107">Methods</span></span>
|<span data-ttu-id="d9854-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d9854-108">Method</span></span>|<span data-ttu-id="d9854-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d9854-109">Return Type</span></span>|<span data-ttu-id="d9854-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9854-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9854-111">DeviceManagementScriptRunSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="d9854-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="d9854-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d9854-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="d9854-113">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d9854-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="d9854-114">DeviceManagementScriptRunSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d9854-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="d9854-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d9854-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="d9854-116">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d9854-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9854-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9854-117">Properties</span></span>
|<span data-ttu-id="d9854-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9854-118">Property</span></span>|<span data-ttu-id="d9854-119">型</span><span class="sxs-lookup"><span data-stu-id="d9854-119">Type</span></span>|<span data-ttu-id="d9854-120">説明</span><span class="sxs-lookup"><span data-stu-id="d9854-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9854-121">id</span><span class="sxs-lookup"><span data-stu-id="d9854-121">id</span></span>|<span data-ttu-id="d9854-122">String</span><span class="sxs-lookup"><span data-stu-id="d9854-122">String</span></span>|<span data-ttu-id="d9854-123">デバイス管理スクリプト実行の概要エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d9854-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="d9854-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9854-124">successDeviceCount</span></span>|<span data-ttu-id="d9854-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d9854-125">Int32</span></span>|<span data-ttu-id="d9854-126">成功したデバイス数。</span><span class="sxs-lookup"><span data-stu-id="d9854-126">Success device count.</span></span>|
|<span data-ttu-id="d9854-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9854-127">errorDeviceCount</span></span>|<span data-ttu-id="d9854-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d9854-128">Int32</span></span>|<span data-ttu-id="d9854-129">エラーデバイス数。</span><span class="sxs-lookup"><span data-stu-id="d9854-129">Error device count.</span></span>|
|<span data-ttu-id="d9854-130">successUserCount</span><span class="sxs-lookup"><span data-stu-id="d9854-130">successUserCount</span></span>|<span data-ttu-id="d9854-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d9854-131">Int32</span></span>|<span data-ttu-id="d9854-132">成功したユーザー数。</span><span class="sxs-lookup"><span data-stu-id="d9854-132">Success user count.</span></span>|
|<span data-ttu-id="d9854-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="d9854-133">errorUserCount</span></span>|<span data-ttu-id="d9854-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d9854-134">Int32</span></span>|<span data-ttu-id="d9854-135">エラーユーザー数。</span><span class="sxs-lookup"><span data-stu-id="d9854-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9854-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d9854-136">Relationships</span></span>
<span data-ttu-id="d9854-137">なし</span><span class="sxs-lookup"><span data-stu-id="d9854-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9854-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9854-138">JSON Representation</span></span>
<span data-ttu-id="d9854-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d9854-139">Here is a JSON representation of the resource.</span></span>
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





