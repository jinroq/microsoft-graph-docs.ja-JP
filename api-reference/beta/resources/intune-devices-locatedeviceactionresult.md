---
title: locateDeviceActionResult リソースの種類
description: デバイスの検索アクションの結果
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 682b2267369a80b3d2cb37d17dd1b2aafdef1f63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416889"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="992b2-103">locateDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="992b2-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="992b2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="992b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="992b2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="992b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="992b2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="992b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="992b2-107">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="992b2-107">Locate device action result</span></span>


<span data-ttu-id="992b2-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="992b2-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="992b2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="992b2-109">Properties</span></span>
|<span data-ttu-id="992b2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="992b2-110">Property</span></span>|<span data-ttu-id="992b2-111">型</span><span class="sxs-lookup"><span data-stu-id="992b2-111">Type</span></span>|<span data-ttu-id="992b2-112">説明</span><span class="sxs-lookup"><span data-stu-id="992b2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="992b2-113">actionName</span><span class="sxs-lookup"><span data-stu-id="992b2-113">actionName</span></span>|<span data-ttu-id="992b2-114">String</span><span class="sxs-lookup"><span data-stu-id="992b2-114">String</span></span>|<span data-ttu-id="992b2-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="992b2-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="992b2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="992b2-116">actionState</span></span>|[<span data-ttu-id="992b2-117">actionState</span><span class="sxs-lookup"><span data-stu-id="992b2-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="992b2-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="992b2-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="992b2-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="992b2-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="992b2-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="992b2-120">startDateTime</span></span>|<span data-ttu-id="992b2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="992b2-121">DateTimeOffset</span></span>|<span data-ttu-id="992b2-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="992b2-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="992b2-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="992b2-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="992b2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="992b2-124">DateTimeOffset</span></span>|<span data-ttu-id="992b2-125">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="992b2-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="992b2-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="992b2-126">deviceLocation</span></span>|[<span data-ttu-id="992b2-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="992b2-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="992b2-128">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="992b2-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="992b2-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="992b2-129">Relationships</span></span>
<span data-ttu-id="992b2-130">なし</span><span class="sxs-lookup"><span data-stu-id="992b2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="992b2-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="992b2-131">JSON Representation</span></span>
<span data-ttu-id="992b2-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="992b2-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
    "lastCollectedDateTimeUtc": "String (timestamp)",
    "lastCollectedDateTime": "String (timestamp)",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "altitude": "<Unknown Primitive Type Edm.Double>",
    "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "heading": "<Unknown Primitive Type Edm.Double>",
    "speed": "<Unknown Primitive Type Edm.Double>"
  }
}
```




