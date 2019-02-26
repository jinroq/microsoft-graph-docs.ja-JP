---
title: windowsDefenderScanActionResult リソースの種類
description: Windows Defender の最後のスキャン結果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20d30ebda6e24f26406d189ebd980e558bf74e83
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251343"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="872fc-103">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="872fc-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="872fc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="872fc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="872fc-105">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="872fc-105">Windows Defender last scan result</span></span>


<span data-ttu-id="872fc-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="872fc-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="872fc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="872fc-107">Properties</span></span>
|<span data-ttu-id="872fc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="872fc-108">Property</span></span>|<span data-ttu-id="872fc-109">型</span><span class="sxs-lookup"><span data-stu-id="872fc-109">Type</span></span>|<span data-ttu-id="872fc-110">説明</span><span class="sxs-lookup"><span data-stu-id="872fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="872fc-111">actionName</span><span class="sxs-lookup"><span data-stu-id="872fc-111">actionName</span></span>|<span data-ttu-id="872fc-112">String</span><span class="sxs-lookup"><span data-stu-id="872fc-112">String</span></span>|<span data-ttu-id="872fc-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="872fc-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="872fc-114">actionState</span><span class="sxs-lookup"><span data-stu-id="872fc-114">actionState</span></span>|[<span data-ttu-id="872fc-115">actionState</span><span class="sxs-lookup"><span data-stu-id="872fc-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="872fc-116">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="872fc-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="872fc-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="872fc-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="872fc-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="872fc-118">startDateTime</span></span>|<span data-ttu-id="872fc-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="872fc-119">DateTimeOffset</span></span>|<span data-ttu-id="872fc-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="872fc-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="872fc-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="872fc-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="872fc-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="872fc-122">DateTimeOffset</span></span>|<span data-ttu-id="872fc-123">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="872fc-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="872fc-124">scanType</span><span class="sxs-lookup"><span data-stu-id="872fc-124">scanType</span></span>|<span data-ttu-id="872fc-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="872fc-125">String</span></span>|<span data-ttu-id="872fc-126">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="872fc-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="872fc-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="872fc-127">Relationships</span></span>
<span data-ttu-id="872fc-128">なし</span><span class="sxs-lookup"><span data-stu-id="872fc-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="872fc-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="872fc-129">JSON Representation</span></span>
<span data-ttu-id="872fc-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="872fc-130">Here is a JSON representation of the resource.</span></span>
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



