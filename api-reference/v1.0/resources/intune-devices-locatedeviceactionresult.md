---
title: locateDeviceActionResult リソースの種類
description: デバイスの検索アクションの結果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69d4eea303711cc5c2174ee05ae97225521ed89f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030745"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="b3d38-103">locateDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3d38-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="b3d38-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3d38-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3d38-105">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="b3d38-105">Locate device action result</span></span>


<span data-ttu-id="b3d38-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b3d38-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3d38-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3d38-107">Properties</span></span>
|<span data-ttu-id="b3d38-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3d38-108">Property</span></span>|<span data-ttu-id="b3d38-109">型</span><span class="sxs-lookup"><span data-stu-id="b3d38-109">Type</span></span>|<span data-ttu-id="b3d38-110">説明</span><span class="sxs-lookup"><span data-stu-id="b3d38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3d38-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b3d38-111">actionName</span></span>|<span data-ttu-id="b3d38-112">String</span><span class="sxs-lookup"><span data-stu-id="b3d38-112">String</span></span>|<span data-ttu-id="b3d38-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="b3d38-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b3d38-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b3d38-114">actionState</span></span>|[<span data-ttu-id="b3d38-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b3d38-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b3d38-116">[Deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="b3d38-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b3d38-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="b3d38-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b3d38-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b3d38-118">startDateTime</span></span>|<span data-ttu-id="b3d38-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3d38-119">DateTimeOffset</span></span>|<span data-ttu-id="b3d38-120">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="b3d38-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b3d38-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3d38-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b3d38-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3d38-122">DateTimeOffset</span></span>|<span data-ttu-id="b3d38-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="b3d38-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b3d38-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="b3d38-124">deviceLocation</span></span>|[<span data-ttu-id="b3d38-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="b3d38-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="b3d38-126">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="b3d38-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3d38-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3d38-127">Relationships</span></span>
<span data-ttu-id="b3d38-128">なし</span><span class="sxs-lookup"><span data-stu-id="b3d38-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3d38-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3d38-129">JSON Representation</span></span>
<span data-ttu-id="b3d38-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3d38-130">Here is a JSON representation of the resource.</span></span>
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



