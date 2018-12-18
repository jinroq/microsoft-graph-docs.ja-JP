---
title: deviceManagementScriptRunSummary リソースの種類
description: デバイス管理スクリプトの実行の概要のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 347a4e5cd3c4201949841054b69c217ad4f9fa8e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338998"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="275db-103">deviceManagementScriptRunSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="275db-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="275db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="275db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="275db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="275db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="275db-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="275db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="275db-107">デバイス管理スクリプトの実行の概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="275db-107">Contains properties for the run summary of a device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="275db-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="275db-108">Methods</span></span>
|<span data-ttu-id="275db-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="275db-109">Method</span></span>|<span data-ttu-id="275db-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="275db-110">Return Type</span></span>|<span data-ttu-id="275db-111">説明</span><span class="sxs-lookup"><span data-stu-id="275db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="275db-112">DeviceManagementScriptRunSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="275db-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="275db-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="275db-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="275db-114">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="275db-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="275db-115">DeviceManagementScriptRunSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="275db-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="275db-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="275db-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="275db-117">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="275db-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="275db-118">Properties</span><span class="sxs-lookup"><span data-stu-id="275db-118">Properties</span></span>
|<span data-ttu-id="275db-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="275db-119">Property</span></span>|<span data-ttu-id="275db-120">種類</span><span class="sxs-lookup"><span data-stu-id="275db-120">Type</span></span>|<span data-ttu-id="275db-121">説明</span><span class="sxs-lookup"><span data-stu-id="275db-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="275db-122">ID</span><span class="sxs-lookup"><span data-stu-id="275db-122">id</span></span>|<span data-ttu-id="275db-123">String</span><span class="sxs-lookup"><span data-stu-id="275db-123">String</span></span>|<span data-ttu-id="275db-124">デバイス管理スクリプトのキーは、エンティティの概要を実行します。</span><span class="sxs-lookup"><span data-stu-id="275db-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="275db-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="275db-125">successDeviceCount</span></span>|<span data-ttu-id="275db-126">Int32</span><span class="sxs-lookup"><span data-stu-id="275db-126">Int32</span></span>|<span data-ttu-id="275db-127">成功した場合のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="275db-127">Success device count.</span></span>|
|<span data-ttu-id="275db-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="275db-128">errorDeviceCount</span></span>|<span data-ttu-id="275db-129">Int32</span><span class="sxs-lookup"><span data-stu-id="275db-129">Int32</span></span>|<span data-ttu-id="275db-130">デバイスのエラーの数です。</span><span class="sxs-lookup"><span data-stu-id="275db-130">Error device count.</span></span>|
|<span data-ttu-id="275db-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="275db-131">successUserCount</span></span>|<span data-ttu-id="275db-132">Int32</span><span class="sxs-lookup"><span data-stu-id="275db-132">Int32</span></span>|<span data-ttu-id="275db-133">成功ユーザー カウントです。</span><span class="sxs-lookup"><span data-stu-id="275db-133">Success user count.</span></span>|
|<span data-ttu-id="275db-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="275db-134">errorUserCount</span></span>|<span data-ttu-id="275db-135">Int32</span><span class="sxs-lookup"><span data-stu-id="275db-135">Int32</span></span>|<span data-ttu-id="275db-136">ユーザーのエラーの数です。</span><span class="sxs-lookup"><span data-stu-id="275db-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="275db-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="275db-137">Relationships</span></span>
<span data-ttu-id="275db-138">なし</span><span class="sxs-lookup"><span data-stu-id="275db-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="275db-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="275db-139">JSON Representation</span></span>
<span data-ttu-id="275db-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="275db-140">Here is a JSON representation of the resource.</span></span>
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





