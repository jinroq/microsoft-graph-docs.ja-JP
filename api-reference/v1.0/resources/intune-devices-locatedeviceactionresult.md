---
title: locateDeviceActionResult リソースの種類
description: デバイスの検索アクションの結果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c335ac49bcf053e58381f7c1111caf5ae70cb0fd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255354"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="35e1e-103">locateDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35e1e-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="35e1e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="35e1e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35e1e-105">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="35e1e-105">Locate device action result</span></span>


<span data-ttu-id="35e1e-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="35e1e-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="35e1e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35e1e-107">Properties</span></span>
|<span data-ttu-id="35e1e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35e1e-108">Property</span></span>|<span data-ttu-id="35e1e-109">型</span><span class="sxs-lookup"><span data-stu-id="35e1e-109">Type</span></span>|<span data-ttu-id="35e1e-110">説明</span><span class="sxs-lookup"><span data-stu-id="35e1e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35e1e-111">actionName</span><span class="sxs-lookup"><span data-stu-id="35e1e-111">actionName</span></span>|<span data-ttu-id="35e1e-112">String</span><span class="sxs-lookup"><span data-stu-id="35e1e-112">String</span></span>|<span data-ttu-id="35e1e-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="35e1e-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="35e1e-114">actionState</span><span class="sxs-lookup"><span data-stu-id="35e1e-114">actionState</span></span>|[<span data-ttu-id="35e1e-115">actionState</span><span class="sxs-lookup"><span data-stu-id="35e1e-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="35e1e-116">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="35e1e-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="35e1e-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="35e1e-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="35e1e-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="35e1e-118">startDateTime</span></span>|<span data-ttu-id="35e1e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35e1e-119">DateTimeOffset</span></span>|<span data-ttu-id="35e1e-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="35e1e-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="35e1e-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="35e1e-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="35e1e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35e1e-122">DateTimeOffset</span></span>|<span data-ttu-id="35e1e-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="35e1e-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="35e1e-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="35e1e-124">deviceLocation</span></span>|[<span data-ttu-id="35e1e-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="35e1e-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="35e1e-126">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="35e1e-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="35e1e-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35e1e-127">Relationships</span></span>
<span data-ttu-id="35e1e-128">なし</span><span class="sxs-lookup"><span data-stu-id="35e1e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35e1e-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35e1e-129">JSON Representation</span></span>
<span data-ttu-id="35e1e-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35e1e-130">Here is a JSON representation of the resource.</span></span>
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



