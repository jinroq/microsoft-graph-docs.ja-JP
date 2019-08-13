---
title: locateDeviceActionResult リソースの種類
description: デバイスの検索アクションの結果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 41992c5b5b1cd4a620d3e2433524478a931b6c7f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372336"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="afde6-103">locateDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="afde6-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="afde6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afde6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afde6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="afde6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afde6-106">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="afde6-106">Locate device action result</span></span>


<span data-ttu-id="afde6-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="afde6-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="afde6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afde6-108">Properties</span></span>
|<span data-ttu-id="afde6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afde6-109">Property</span></span>|<span data-ttu-id="afde6-110">型</span><span class="sxs-lookup"><span data-stu-id="afde6-110">Type</span></span>|<span data-ttu-id="afde6-111">説明</span><span class="sxs-lookup"><span data-stu-id="afde6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afde6-112">actionName</span><span class="sxs-lookup"><span data-stu-id="afde6-112">actionName</span></span>|<span data-ttu-id="afde6-113">String</span><span class="sxs-lookup"><span data-stu-id="afde6-113">String</span></span>|<span data-ttu-id="afde6-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="afde6-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="afde6-115">actionState</span><span class="sxs-lookup"><span data-stu-id="afde6-115">actionState</span></span>|[<span data-ttu-id="afde6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="afde6-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="afde6-117">[Deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="afde6-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="afde6-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="afde6-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="afde6-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="afde6-119">startDateTime</span></span>|<span data-ttu-id="afde6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afde6-120">DateTimeOffset</span></span>|<span data-ttu-id="afde6-121">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="afde6-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="afde6-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="afde6-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="afde6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afde6-123">DateTimeOffset</span></span>|<span data-ttu-id="afde6-124">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="afde6-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="afde6-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="afde6-125">deviceLocation</span></span>|[<span data-ttu-id="afde6-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="afde6-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="afde6-127">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="afde6-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="afde6-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="afde6-128">Relationships</span></span>
<span data-ttu-id="afde6-129">なし</span><span class="sxs-lookup"><span data-stu-id="afde6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="afde6-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="afde6-130">JSON Representation</span></span>
<span data-ttu-id="afde6-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="afde6-131">Here is a JSON representation of the resource.</span></span>
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



