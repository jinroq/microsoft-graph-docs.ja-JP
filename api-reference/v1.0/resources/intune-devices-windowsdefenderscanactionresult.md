---
title: windowsDefenderScanActionResult リソースの種類
description: Windows Defender の最後のスキャン結果
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a323b0438c7edf50d745b3b21498ad5c50f6424
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911687"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="c6cae-103">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6cae-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="c6cae-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6cae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6cae-105">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="c6cae-105">Windows Defender last scan result</span></span>

<span data-ttu-id="c6cae-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c6cae-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c6cae-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6cae-107">Properties</span></span>
|<span data-ttu-id="c6cae-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6cae-108">Property</span></span>|<span data-ttu-id="c6cae-109">種類</span><span class="sxs-lookup"><span data-stu-id="c6cae-109">Type</span></span>|<span data-ttu-id="c6cae-110">説明</span><span class="sxs-lookup"><span data-stu-id="c6cae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6cae-111">actionName</span><span class="sxs-lookup"><span data-stu-id="c6cae-111">actionName</span></span>|<span data-ttu-id="c6cae-112">String</span><span class="sxs-lookup"><span data-stu-id="c6cae-112">String</span></span>|<span data-ttu-id="c6cae-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="c6cae-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c6cae-114">actionState</span><span class="sxs-lookup"><span data-stu-id="c6cae-114">actionState</span></span>|[<span data-ttu-id="c6cae-115">actionState</span><span class="sxs-lookup"><span data-stu-id="c6cae-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="c6cae-116">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="c6cae-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c6cae-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="c6cae-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c6cae-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c6cae-118">startDateTime</span></span>|<span data-ttu-id="c6cae-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6cae-119">DateTimeOffset</span></span>|<span data-ttu-id="c6cae-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c6cae-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c6cae-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6cae-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="c6cae-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6cae-122">DateTimeOffset</span></span>|<span data-ttu-id="c6cae-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="c6cae-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c6cae-124">scanType</span><span class="sxs-lookup"><span data-stu-id="c6cae-124">scanType</span></span>|<span data-ttu-id="c6cae-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c6cae-125">String</span></span>|<span data-ttu-id="c6cae-126">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="c6cae-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6cae-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6cae-127">Relationships</span></span>
<span data-ttu-id="c6cae-128">なし</span><span class="sxs-lookup"><span data-stu-id="c6cae-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6cae-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6cae-129">JSON Representation</span></span>
<span data-ttu-id="c6cae-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c6cae-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



