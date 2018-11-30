---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
ms.openlocfilehash: 1a543f21d1f82b9f2bee0f004d3b8fab88c863b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022498"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="5d4b0-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d4b0-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="5d4b0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d4b0-105">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="5d4b0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d4b0-106">Properties</span></span>
|<span data-ttu-id="5d4b0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d4b0-107">Property</span></span>|<span data-ttu-id="5d4b0-108">型</span><span class="sxs-lookup"><span data-stu-id="5d4b0-108">Type</span></span>|<span data-ttu-id="5d4b0-109">説明</span><span class="sxs-lookup"><span data-stu-id="5d4b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d4b0-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="5d4b0-110">androidCount</span></span>|<span data-ttu-id="5d4b0-111">Int32</span><span class="sxs-lookup"><span data-stu-id="5d4b0-111">Int32</span></span>|<span data-ttu-id="5d4b0-112">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-112">Number of android device count.</span></span>|
|<span data-ttu-id="5d4b0-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="5d4b0-113">iosCount</span></span>|<span data-ttu-id="5d4b0-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5d4b0-114">Int32</span></span>|<span data-ttu-id="5d4b0-115">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="5d4b0-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="5d4b0-116">macOSCount</span></span>|<span data-ttu-id="5d4b0-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5d4b0-117">Int32</span></span>|<span data-ttu-id="5d4b0-118">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="5d4b0-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="5d4b0-119">windowsMobileCount</span></span>|<span data-ttu-id="5d4b0-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5d4b0-120">Int32</span></span>|<span data-ttu-id="5d4b0-121">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="5d4b0-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="5d4b0-122">windowsCount</span></span>|<span data-ttu-id="5d4b0-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5d4b0-123">Int32</span></span>|<span data-ttu-id="5d4b0-124">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="5d4b0-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="5d4b0-125">unknownCount</span></span>|<span data-ttu-id="5d4b0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5d4b0-126">Int32</span></span>|<span data-ttu-id="5d4b0-127">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d4b0-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5d4b0-128">Relationships</span></span>
<span data-ttu-id="5d4b0-129">なし</span><span class="sxs-lookup"><span data-stu-id="5d4b0-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d4b0-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d4b0-130">JSON Representation</span></span>
<span data-ttu-id="5d4b0-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5d4b0-131">Here is a JSON representation of the resource.</span></span>
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


