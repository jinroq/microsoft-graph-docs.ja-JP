---
title: deviceManagementScriptRunSummary リソースの種類
description: デバイス管理スクリプトの実行の概要のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2109822ce081fc18286722cb48209a4349aa2b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823542"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="f3d61-103">deviceManagementScriptRunSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3d61-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="f3d61-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3d61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3d61-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3d61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3d61-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3d61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3d61-107">デバイス管理スクリプトの実行の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3d61-107">Contains properties for the run summary of a device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="f3d61-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f3d61-108">Methods</span></span>
|<span data-ttu-id="f3d61-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f3d61-109">Method</span></span>|<span data-ttu-id="f3d61-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f3d61-110">Return Type</span></span>|<span data-ttu-id="f3d61-111">説明</span><span class="sxs-lookup"><span data-stu-id="f3d61-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3d61-112">DeviceManagementScriptRunSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="f3d61-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="f3d61-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="f3d61-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="f3d61-114">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3d61-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="f3d61-115">DeviceManagementScriptRunSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="f3d61-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="f3d61-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="f3d61-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="f3d61-117">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3d61-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3d61-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3d61-118">Properties</span></span>
|<span data-ttu-id="f3d61-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3d61-119">Property</span></span>|<span data-ttu-id="f3d61-120">種類</span><span class="sxs-lookup"><span data-stu-id="f3d61-120">Type</span></span>|<span data-ttu-id="f3d61-121">説明</span><span class="sxs-lookup"><span data-stu-id="f3d61-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3d61-122">ID</span><span class="sxs-lookup"><span data-stu-id="f3d61-122">id</span></span>|<span data-ttu-id="f3d61-123">String</span><span class="sxs-lookup"><span data-stu-id="f3d61-123">String</span></span>|<span data-ttu-id="f3d61-124">デバイス管理スクリプトのキーは、エンティティの概要を実行します。</span><span class="sxs-lookup"><span data-stu-id="f3d61-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="f3d61-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3d61-125">successDeviceCount</span></span>|<span data-ttu-id="f3d61-126">Int32</span><span class="sxs-lookup"><span data-stu-id="f3d61-126">Int32</span></span>|<span data-ttu-id="f3d61-127">成功した場合のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="f3d61-127">Success device count.</span></span>|
|<span data-ttu-id="f3d61-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3d61-128">errorDeviceCount</span></span>|<span data-ttu-id="f3d61-129">Int32</span><span class="sxs-lookup"><span data-stu-id="f3d61-129">Int32</span></span>|<span data-ttu-id="f3d61-130">デバイスのエラーの数です。</span><span class="sxs-lookup"><span data-stu-id="f3d61-130">Error device count.</span></span>|
|<span data-ttu-id="f3d61-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="f3d61-131">successUserCount</span></span>|<span data-ttu-id="f3d61-132">Int32</span><span class="sxs-lookup"><span data-stu-id="f3d61-132">Int32</span></span>|<span data-ttu-id="f3d61-133">成功ユーザー カウントです。</span><span class="sxs-lookup"><span data-stu-id="f3d61-133">Success user count.</span></span>|
|<span data-ttu-id="f3d61-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="f3d61-134">errorUserCount</span></span>|<span data-ttu-id="f3d61-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f3d61-135">Int32</span></span>|<span data-ttu-id="f3d61-136">ユーザーのエラーの数です。</span><span class="sxs-lookup"><span data-stu-id="f3d61-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3d61-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3d61-137">Relationships</span></span>
<span data-ttu-id="f3d61-138">なし</span><span class="sxs-lookup"><span data-stu-id="f3d61-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3d61-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3d61-139">JSON Representation</span></span>
<span data-ttu-id="f3d61-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3d61-140">Here is a JSON representation of the resource.</span></span>
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





