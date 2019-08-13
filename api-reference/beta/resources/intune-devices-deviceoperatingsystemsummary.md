---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a9e628a52a90f72dbf67495c8e6745bd4072ca2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369984"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="e4130-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4130-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="e4130-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4130-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4130-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e4130-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4130-106">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="e4130-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="e4130-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4130-107">Properties</span></span>
|<span data-ttu-id="e4130-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4130-108">Property</span></span>|<span data-ttu-id="e4130-109">型</span><span class="sxs-lookup"><span data-stu-id="e4130-109">Type</span></span>|<span data-ttu-id="e4130-110">説明</span><span class="sxs-lookup"><span data-stu-id="e4130-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4130-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="e4130-111">androidCount</span></span>|<span data-ttu-id="e4130-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e4130-112">Int32</span></span>|<span data-ttu-id="e4130-113">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e4130-113">Number of android device count.</span></span>|
|<span data-ttu-id="e4130-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="e4130-114">iosCount</span></span>|<span data-ttu-id="e4130-115">Int32</span><span class="sxs-lookup"><span data-stu-id="e4130-115">Int32</span></span>|<span data-ttu-id="e4130-116">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e4130-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="e4130-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="e4130-117">macOSCount</span></span>|<span data-ttu-id="e4130-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e4130-118">Int32</span></span>|<span data-ttu-id="e4130-119">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e4130-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="e4130-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="e4130-120">windowsMobileCount</span></span>|<span data-ttu-id="e4130-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e4130-121">Int32</span></span>|<span data-ttu-id="e4130-122">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e4130-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="e4130-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="e4130-123">windowsCount</span></span>|<span data-ttu-id="e4130-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e4130-124">Int32</span></span>|<span data-ttu-id="e4130-125">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e4130-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="e4130-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="e4130-126">unknownCount</span></span>|<span data-ttu-id="e4130-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e4130-127">Int32</span></span>|<span data-ttu-id="e4130-128">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="e4130-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4130-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e4130-129">Relationships</span></span>
<span data-ttu-id="e4130-130">なし</span><span class="sxs-lookup"><span data-stu-id="e4130-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4130-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4130-131">JSON Representation</span></span>
<span data-ttu-id="e4130-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e4130-132">Here is a JSON representation of the resource.</span></span>
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



