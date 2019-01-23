---
title: windowsDefenderScanActionResult リソースの種類
description: Windows Defender の最後のスキャン結果
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 913c821b60feb4901d812f2055c72e028537dd12
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405500"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="fbe49-103">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbe49-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="fbe49-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fbe49-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fbe49-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbe49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbe49-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fbe49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbe49-107">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="fbe49-107">Windows Defender last scan result</span></span>


<span data-ttu-id="fbe49-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="fbe49-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbe49-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbe49-109">Properties</span></span>
|<span data-ttu-id="fbe49-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbe49-110">Property</span></span>|<span data-ttu-id="fbe49-111">型</span><span class="sxs-lookup"><span data-stu-id="fbe49-111">Type</span></span>|<span data-ttu-id="fbe49-112">説明</span><span class="sxs-lookup"><span data-stu-id="fbe49-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbe49-113">actionName</span><span class="sxs-lookup"><span data-stu-id="fbe49-113">actionName</span></span>|<span data-ttu-id="fbe49-114">String</span><span class="sxs-lookup"><span data-stu-id="fbe49-114">String</span></span>|<span data-ttu-id="fbe49-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="fbe49-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fbe49-116">actionState</span><span class="sxs-lookup"><span data-stu-id="fbe49-116">actionState</span></span>|[<span data-ttu-id="fbe49-117">actionState</span><span class="sxs-lookup"><span data-stu-id="fbe49-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fbe49-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="fbe49-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="fbe49-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="fbe49-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fbe49-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fbe49-120">startDateTime</span></span>|<span data-ttu-id="fbe49-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbe49-121">DateTimeOffset</span></span>|<span data-ttu-id="fbe49-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fbe49-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fbe49-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbe49-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="fbe49-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbe49-124">DateTimeOffset</span></span>|<span data-ttu-id="fbe49-125">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="fbe49-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fbe49-126">scanType</span><span class="sxs-lookup"><span data-stu-id="fbe49-126">scanType</span></span>|<span data-ttu-id="fbe49-127">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fbe49-127">String</span></span>|<span data-ttu-id="fbe49-128">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="fbe49-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbe49-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbe49-129">Relationships</span></span>
<span data-ttu-id="fbe49-130">なし</span><span class="sxs-lookup"><span data-stu-id="fbe49-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbe49-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbe49-131">JSON Representation</span></span>
<span data-ttu-id="fbe49-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fbe49-132">Here is a JSON representation of the resource.</span></span>
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




