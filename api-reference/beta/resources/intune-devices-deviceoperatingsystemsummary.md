---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
author: tfitzmac
ms.openlocfilehash: 8dd3bf85a75d5acf6ae4bb0cecb8fd360c4e0459
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341861"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="643be-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="643be-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="643be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="643be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="643be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="643be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="643be-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="643be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="643be-107">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="643be-107">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="643be-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="643be-108">Properties</span></span>
|<span data-ttu-id="643be-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="643be-109">Property</span></span>|<span data-ttu-id="643be-110">種類</span><span class="sxs-lookup"><span data-stu-id="643be-110">Type</span></span>|<span data-ttu-id="643be-111">説明</span><span class="sxs-lookup"><span data-stu-id="643be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="643be-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="643be-112">androidCount</span></span>|<span data-ttu-id="643be-113">Int32</span><span class="sxs-lookup"><span data-stu-id="643be-113">Int32</span></span>|<span data-ttu-id="643be-114">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="643be-114">Number of android device count.</span></span>|
|<span data-ttu-id="643be-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="643be-115">iosCount</span></span>|<span data-ttu-id="643be-116">Int32</span><span class="sxs-lookup"><span data-stu-id="643be-116">Int32</span></span>|<span data-ttu-id="643be-117">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="643be-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="643be-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="643be-118">macOSCount</span></span>|<span data-ttu-id="643be-119">Int32</span><span class="sxs-lookup"><span data-stu-id="643be-119">Int32</span></span>|<span data-ttu-id="643be-120">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="643be-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="643be-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="643be-121">windowsMobileCount</span></span>|<span data-ttu-id="643be-122">Int32</span><span class="sxs-lookup"><span data-stu-id="643be-122">Int32</span></span>|<span data-ttu-id="643be-123">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="643be-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="643be-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="643be-124">windowsCount</span></span>|<span data-ttu-id="643be-125">Int32</span><span class="sxs-lookup"><span data-stu-id="643be-125">Int32</span></span>|<span data-ttu-id="643be-126">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="643be-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="643be-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="643be-127">unknownCount</span></span>|<span data-ttu-id="643be-128">Int32</span><span class="sxs-lookup"><span data-stu-id="643be-128">Int32</span></span>|<span data-ttu-id="643be-129">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="643be-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="643be-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="643be-130">Relationships</span></span>
<span data-ttu-id="643be-131">なし</span><span class="sxs-lookup"><span data-stu-id="643be-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="643be-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="643be-132">JSON Representation</span></span>
<span data-ttu-id="643be-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="643be-133">Here is a JSON representation of the resource.</span></span>
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





