---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c806e250d6b201e6dfe49d90685c4144913182
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250405"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="f2912-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2912-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="f2912-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2912-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2912-105">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="f2912-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="f2912-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2912-106">Properties</span></span>
|<span data-ttu-id="f2912-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2912-107">Property</span></span>|<span data-ttu-id="f2912-108">型</span><span class="sxs-lookup"><span data-stu-id="f2912-108">Type</span></span>|<span data-ttu-id="f2912-109">説明</span><span class="sxs-lookup"><span data-stu-id="f2912-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2912-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="f2912-110">androidCount</span></span>|<span data-ttu-id="f2912-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f2912-111">Int32</span></span>|<span data-ttu-id="f2912-112">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f2912-112">Number of android device count.</span></span>|
|<span data-ttu-id="f2912-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="f2912-113">iosCount</span></span>|<span data-ttu-id="f2912-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f2912-114">Int32</span></span>|<span data-ttu-id="f2912-115">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f2912-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="f2912-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="f2912-116">macOSCount</span></span>|<span data-ttu-id="f2912-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f2912-117">Int32</span></span>|<span data-ttu-id="f2912-118">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f2912-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="f2912-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="f2912-119">windowsMobileCount</span></span>|<span data-ttu-id="f2912-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f2912-120">Int32</span></span>|<span data-ttu-id="f2912-121">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f2912-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="f2912-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="f2912-122">windowsCount</span></span>|<span data-ttu-id="f2912-123">Int32</span><span class="sxs-lookup"><span data-stu-id="f2912-123">Int32</span></span>|<span data-ttu-id="f2912-124">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f2912-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="f2912-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="f2912-125">unknownCount</span></span>|<span data-ttu-id="f2912-126">Int32</span><span class="sxs-lookup"><span data-stu-id="f2912-126">Int32</span></span>|<span data-ttu-id="f2912-127">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f2912-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2912-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2912-128">Relationships</span></span>
<span data-ttu-id="f2912-129">なし</span><span class="sxs-lookup"><span data-stu-id="f2912-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2912-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2912-130">JSON Representation</span></span>
<span data-ttu-id="f2912-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2912-131">Here is a JSON representation of the resource.</span></span>
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



