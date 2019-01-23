---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 009998d495eb033510bbc27437b72f866fd4ed7e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410771"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="c8b8a-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8b8a-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="c8b8a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8b8a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8b8a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8b8a-107">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="c8b8a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8b8a-108">Properties</span></span>
|<span data-ttu-id="c8b8a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8b8a-109">Property</span></span>|<span data-ttu-id="c8b8a-110">型</span><span class="sxs-lookup"><span data-stu-id="c8b8a-110">Type</span></span>|<span data-ttu-id="c8b8a-111">説明</span><span class="sxs-lookup"><span data-stu-id="c8b8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8b8a-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="c8b8a-112">androidCount</span></span>|<span data-ttu-id="c8b8a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c8b8a-113">Int32</span></span>|<span data-ttu-id="c8b8a-114">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-114">Number of android device count.</span></span>|
|<span data-ttu-id="c8b8a-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="c8b8a-115">iosCount</span></span>|<span data-ttu-id="c8b8a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c8b8a-116">Int32</span></span>|<span data-ttu-id="c8b8a-117">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="c8b8a-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="c8b8a-118">macOSCount</span></span>|<span data-ttu-id="c8b8a-119">Int32</span><span class="sxs-lookup"><span data-stu-id="c8b8a-119">Int32</span></span>|<span data-ttu-id="c8b8a-120">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="c8b8a-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="c8b8a-121">windowsMobileCount</span></span>|<span data-ttu-id="c8b8a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c8b8a-122">Int32</span></span>|<span data-ttu-id="c8b8a-123">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="c8b8a-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="c8b8a-124">windowsCount</span></span>|<span data-ttu-id="c8b8a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c8b8a-125">Int32</span></span>|<span data-ttu-id="c8b8a-126">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="c8b8a-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="c8b8a-127">unknownCount</span></span>|<span data-ttu-id="c8b8a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c8b8a-128">Int32</span></span>|<span data-ttu-id="c8b8a-129">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8b8a-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8b8a-130">Relationships</span></span>
<span data-ttu-id="c8b8a-131">なし</span><span class="sxs-lookup"><span data-stu-id="c8b8a-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8b8a-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8b8a-132">JSON Representation</span></span>
<span data-ttu-id="c8b8a-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8b8a-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```




