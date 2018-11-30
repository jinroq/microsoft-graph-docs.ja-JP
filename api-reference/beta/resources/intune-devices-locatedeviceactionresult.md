---
title: locateDeviceActionResult リソースの種類
description: デバイスの検索アクションの結果
ms.openlocfilehash: de7a59826478f8e11cf44635dcc4e437b60d7e83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074257"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="e7ddb-103">locateDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7ddb-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="e7ddb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e7ddb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7ddb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7ddb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7ddb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7ddb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7ddb-107">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="e7ddb-107">Locate device action result</span></span>

<span data-ttu-id="e7ddb-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e7ddb-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e7ddb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7ddb-109">Properties</span></span>
|<span data-ttu-id="e7ddb-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7ddb-110">Property</span></span>|<span data-ttu-id="e7ddb-111">型</span><span class="sxs-lookup"><span data-stu-id="e7ddb-111">Type</span></span>|<span data-ttu-id="e7ddb-112">説明</span><span class="sxs-lookup"><span data-stu-id="e7ddb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7ddb-113">actionName</span><span class="sxs-lookup"><span data-stu-id="e7ddb-113">actionName</span></span>|<span data-ttu-id="e7ddb-114">String</span><span class="sxs-lookup"><span data-stu-id="e7ddb-114">String</span></span>|<span data-ttu-id="e7ddb-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="e7ddb-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e7ddb-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e7ddb-116">actionState</span></span>|[<span data-ttu-id="e7ddb-117">actionState</span><span class="sxs-lookup"><span data-stu-id="e7ddb-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e7ddb-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="e7ddb-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e7ddb-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="e7ddb-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e7ddb-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ddb-120">startDateTime</span></span>|<span data-ttu-id="e7ddb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ddb-121">DateTimeOffset</span></span>|<span data-ttu-id="e7ddb-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e7ddb-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e7ddb-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ddb-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="e7ddb-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ddb-124">DateTimeOffset</span></span>|<span data-ttu-id="e7ddb-125">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="e7ddb-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e7ddb-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="e7ddb-126">deviceLocation</span></span>|[<span data-ttu-id="e7ddb-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="e7ddb-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="e7ddb-128">デバイスの場所</span><span class="sxs-lookup"><span data-stu-id="e7ddb-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7ddb-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7ddb-129">Relationships</span></span>
<span data-ttu-id="e7ddb-130">なし</span><span class="sxs-lookup"><span data-stu-id="e7ddb-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7ddb-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7ddb-131">JSON Representation</span></span>
<span data-ttu-id="e7ddb-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7ddb-132">Here is a JSON representation of the resource.</span></span>
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





