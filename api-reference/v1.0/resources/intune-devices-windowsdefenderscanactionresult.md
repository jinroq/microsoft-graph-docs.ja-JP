---
title: windowsDefenderScanActionResult リソースの種類
description: Windows Defender の最後のスキャン結果
ms.openlocfilehash: 6221e0d746e677f09b2be00ec66a898e6dfc288c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020591"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="880ef-103">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="880ef-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="880ef-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="880ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="880ef-105">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="880ef-105">Windows Defender last scan result</span></span>

<span data-ttu-id="880ef-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="880ef-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="880ef-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="880ef-107">Properties</span></span>
|<span data-ttu-id="880ef-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="880ef-108">Property</span></span>|<span data-ttu-id="880ef-109">型</span><span class="sxs-lookup"><span data-stu-id="880ef-109">Type</span></span>|<span data-ttu-id="880ef-110">説明</span><span class="sxs-lookup"><span data-stu-id="880ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="880ef-111">actionName</span><span class="sxs-lookup"><span data-stu-id="880ef-111">actionName</span></span>|<span data-ttu-id="880ef-112">String</span><span class="sxs-lookup"><span data-stu-id="880ef-112">String</span></span>|<span data-ttu-id="880ef-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="880ef-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="880ef-114">actionState</span><span class="sxs-lookup"><span data-stu-id="880ef-114">actionState</span></span>|[<span data-ttu-id="880ef-115">actionState</span><span class="sxs-lookup"><span data-stu-id="880ef-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="880ef-116">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="880ef-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="880ef-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="880ef-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="880ef-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="880ef-118">startDateTime</span></span>|<span data-ttu-id="880ef-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="880ef-119">DateTimeOffset</span></span>|<span data-ttu-id="880ef-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="880ef-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="880ef-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="880ef-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="880ef-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="880ef-122">DateTimeOffset</span></span>|<span data-ttu-id="880ef-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="880ef-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="880ef-124">scanType</span><span class="sxs-lookup"><span data-stu-id="880ef-124">scanType</span></span>|<span data-ttu-id="880ef-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="880ef-125">String</span></span>|<span data-ttu-id="880ef-126">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="880ef-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="880ef-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="880ef-127">Relationships</span></span>
<span data-ttu-id="880ef-128">なし</span><span class="sxs-lookup"><span data-stu-id="880ef-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="880ef-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="880ef-129">JSON Representation</span></span>
<span data-ttu-id="880ef-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="880ef-130">Here is a JSON representation of the resource.</span></span>
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



