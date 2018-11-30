---
title: locateDeviceActionResult リソースの種類
description: デバイスの検索アクションの結果
ms.openlocfilehash: 3cabeca1ac07dd1911cf4c60300d07bdc1266134
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021922"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="6be87-103">locateDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6be87-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="6be87-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6be87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6be87-105">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="6be87-105">Locate device action result</span></span>

<span data-ttu-id="6be87-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6be87-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6be87-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6be87-107">Properties</span></span>
|<span data-ttu-id="6be87-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6be87-108">Property</span></span>|<span data-ttu-id="6be87-109">型</span><span class="sxs-lookup"><span data-stu-id="6be87-109">Type</span></span>|<span data-ttu-id="6be87-110">説明</span><span class="sxs-lookup"><span data-stu-id="6be87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6be87-111">actionName</span><span class="sxs-lookup"><span data-stu-id="6be87-111">actionName</span></span>|<span data-ttu-id="6be87-112">String</span><span class="sxs-lookup"><span data-stu-id="6be87-112">String</span></span>|<span data-ttu-id="6be87-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="6be87-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6be87-114">actionState</span><span class="sxs-lookup"><span data-stu-id="6be87-114">actionState</span></span>|[<span data-ttu-id="6be87-115">actionState</span><span class="sxs-lookup"><span data-stu-id="6be87-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="6be87-116">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="6be87-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="6be87-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="6be87-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6be87-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6be87-118">startDateTime</span></span>|<span data-ttu-id="6be87-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6be87-119">DateTimeOffset</span></span>|<span data-ttu-id="6be87-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="6be87-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6be87-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6be87-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="6be87-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6be87-122">DateTimeOffset</span></span>|<span data-ttu-id="6be87-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="6be87-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6be87-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="6be87-124">deviceLocation</span></span>|[<span data-ttu-id="6be87-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="6be87-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="6be87-126">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="6be87-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="6be87-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6be87-127">Relationships</span></span>
<span data-ttu-id="6be87-128">なし</span><span class="sxs-lookup"><span data-stu-id="6be87-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6be87-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6be87-129">JSON Representation</span></span>
<span data-ttu-id="6be87-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6be87-130">Here is a JSON representation of the resource.</span></span>
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



