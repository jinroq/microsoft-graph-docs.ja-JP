---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d53d9fdfcf3dfcc86f40ccadb3d71bdbd6b8686b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942039"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="4f3a0-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f3a0-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="4f3a0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f3a0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f3a0-106">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="4f3a0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f3a0-107">Properties</span></span>
|<span data-ttu-id="4f3a0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f3a0-108">Property</span></span>|<span data-ttu-id="4f3a0-109">型</span><span class="sxs-lookup"><span data-stu-id="4f3a0-109">Type</span></span>|<span data-ttu-id="4f3a0-110">説明</span><span class="sxs-lookup"><span data-stu-id="4f3a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f3a0-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="4f3a0-111">androidCount</span></span>|<span data-ttu-id="4f3a0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="4f3a0-112">Int32</span></span>|<span data-ttu-id="4f3a0-113">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-113">Number of android device count.</span></span>|
|<span data-ttu-id="4f3a0-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="4f3a0-114">iosCount</span></span>|<span data-ttu-id="4f3a0-115">Int32</span><span class="sxs-lookup"><span data-stu-id="4f3a0-115">Int32</span></span>|<span data-ttu-id="4f3a0-116">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="4f3a0-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="4f3a0-117">macOSCount</span></span>|<span data-ttu-id="4f3a0-118">Int32</span><span class="sxs-lookup"><span data-stu-id="4f3a0-118">Int32</span></span>|<span data-ttu-id="4f3a0-119">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="4f3a0-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="4f3a0-120">windowsMobileCount</span></span>|<span data-ttu-id="4f3a0-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4f3a0-121">Int32</span></span>|<span data-ttu-id="4f3a0-122">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="4f3a0-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="4f3a0-123">windowsCount</span></span>|<span data-ttu-id="4f3a0-124">Int32</span><span class="sxs-lookup"><span data-stu-id="4f3a0-124">Int32</span></span>|<span data-ttu-id="4f3a0-125">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="4f3a0-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="4f3a0-126">unknownCount</span></span>|<span data-ttu-id="4f3a0-127">Int32</span><span class="sxs-lookup"><span data-stu-id="4f3a0-127">Int32</span></span>|<span data-ttu-id="4f3a0-128">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f3a0-129">関係</span><span class="sxs-lookup"><span data-stu-id="4f3a0-129">Relationships</span></span>
<span data-ttu-id="4f3a0-130">なし</span><span class="sxs-lookup"><span data-stu-id="4f3a0-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f3a0-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f3a0-131">JSON Representation</span></span>
<span data-ttu-id="4f3a0-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4f3a0-132">Here is a JSON representation of the resource.</span></span>
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




