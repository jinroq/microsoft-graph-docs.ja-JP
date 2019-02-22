---
title: windowsDefenderScanActionResult リソースの種類
description: Windows Defender の最後のスキャン結果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 094880247ee2612d0066bb44aa6f6bb581f7efe5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148644"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="4e191-103">windowsDefenderScanActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e191-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="4e191-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e191-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e191-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e191-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e191-106">Windows Defender の最後のスキャン結果</span><span class="sxs-lookup"><span data-stu-id="4e191-106">Windows Defender last scan result</span></span>


<span data-ttu-id="4e191-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4e191-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e191-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e191-108">Properties</span></span>
|<span data-ttu-id="4e191-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e191-109">Property</span></span>|<span data-ttu-id="4e191-110">型</span><span class="sxs-lookup"><span data-stu-id="4e191-110">Type</span></span>|<span data-ttu-id="4e191-111">説明</span><span class="sxs-lookup"><span data-stu-id="4e191-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e191-112">actionName</span><span class="sxs-lookup"><span data-stu-id="4e191-112">actionName</span></span>|<span data-ttu-id="4e191-113">String</span><span class="sxs-lookup"><span data-stu-id="4e191-113">String</span></span>|<span data-ttu-id="4e191-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="4e191-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e191-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4e191-115">actionState</span></span>|[<span data-ttu-id="4e191-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4e191-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4e191-117">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="4e191-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4e191-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="4e191-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4e191-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e191-119">startDateTime</span></span>|<span data-ttu-id="4e191-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e191-120">DateTimeOffset</span></span>|<span data-ttu-id="4e191-121">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4e191-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e191-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e191-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="4e191-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e191-123">DateTimeOffset</span></span>|<span data-ttu-id="4e191-124">アクション状態の最終更新時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承</span><span class="sxs-lookup"><span data-stu-id="4e191-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e191-125">scanType</span><span class="sxs-lookup"><span data-stu-id="4e191-125">scanType</span></span>|<span data-ttu-id="4e191-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4e191-126">String</span></span>|<span data-ttu-id="4e191-127">スキャンの種類。フル スキャンまたはクイック スキャン</span><span class="sxs-lookup"><span data-stu-id="4e191-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e191-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4e191-128">Relationships</span></span>
<span data-ttu-id="4e191-129">なし</span><span class="sxs-lookup"><span data-stu-id="4e191-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e191-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e191-130">JSON Representation</span></span>
<span data-ttu-id="4e191-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4e191-131">Here is a JSON representation of the resource.</span></span>
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




