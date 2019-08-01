---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9877dba58817e8c6dad3676cb6a646750408d4e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030759"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="4d5a4-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d5a4-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="4d5a4-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d5a4-105">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="4d5a4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d5a4-106">Properties</span></span>
|<span data-ttu-id="4d5a4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d5a4-107">Property</span></span>|<span data-ttu-id="4d5a4-108">型</span><span class="sxs-lookup"><span data-stu-id="4d5a4-108">Type</span></span>|<span data-ttu-id="4d5a4-109">説明</span><span class="sxs-lookup"><span data-stu-id="4d5a4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d5a4-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="4d5a4-110">androidCount</span></span>|<span data-ttu-id="4d5a4-111">Int32</span><span class="sxs-lookup"><span data-stu-id="4d5a4-111">Int32</span></span>|<span data-ttu-id="4d5a4-112">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-112">Number of android device count.</span></span>|
|<span data-ttu-id="4d5a4-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="4d5a4-113">iosCount</span></span>|<span data-ttu-id="4d5a4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="4d5a4-114">Int32</span></span>|<span data-ttu-id="4d5a4-115">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="4d5a4-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="4d5a4-116">macOSCount</span></span>|<span data-ttu-id="4d5a4-117">Int32</span><span class="sxs-lookup"><span data-stu-id="4d5a4-117">Int32</span></span>|<span data-ttu-id="4d5a4-118">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="4d5a4-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="4d5a4-119">windowsMobileCount</span></span>|<span data-ttu-id="4d5a4-120">Int32</span><span class="sxs-lookup"><span data-stu-id="4d5a4-120">Int32</span></span>|<span data-ttu-id="4d5a4-121">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="4d5a4-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="4d5a4-122">windowsCount</span></span>|<span data-ttu-id="4d5a4-123">Int32</span><span class="sxs-lookup"><span data-stu-id="4d5a4-123">Int32</span></span>|<span data-ttu-id="4d5a4-124">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="4d5a4-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="4d5a4-125">unknownCount</span></span>|<span data-ttu-id="4d5a4-126">Int32</span><span class="sxs-lookup"><span data-stu-id="4d5a4-126">Int32</span></span>|<span data-ttu-id="4d5a4-127">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d5a4-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4d5a4-128">Relationships</span></span>
<span data-ttu-id="4d5a4-129">なし</span><span class="sxs-lookup"><span data-stu-id="4d5a4-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d5a4-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d5a4-130">JSON Representation</span></span>
<span data-ttu-id="4d5a4-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4d5a4-131">Here is a JSON representation of the resource.</span></span>
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



