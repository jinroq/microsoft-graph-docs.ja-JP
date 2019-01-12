---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2147034c060fa15e8e799d5ddbe72aabe635af08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975646"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="39dc4-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39dc4-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="39dc4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="39dc4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39dc4-105">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="39dc4-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="39dc4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39dc4-106">Properties</span></span>
|<span data-ttu-id="39dc4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39dc4-107">Property</span></span>|<span data-ttu-id="39dc4-108">種類</span><span class="sxs-lookup"><span data-stu-id="39dc4-108">Type</span></span>|<span data-ttu-id="39dc4-109">説明</span><span class="sxs-lookup"><span data-stu-id="39dc4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39dc4-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="39dc4-110">androidCount</span></span>|<span data-ttu-id="39dc4-111">Int32</span><span class="sxs-lookup"><span data-stu-id="39dc4-111">Int32</span></span>|<span data-ttu-id="39dc4-112">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39dc4-112">Number of android device count.</span></span>|
|<span data-ttu-id="39dc4-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="39dc4-113">iosCount</span></span>|<span data-ttu-id="39dc4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="39dc4-114">Int32</span></span>|<span data-ttu-id="39dc4-115">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39dc4-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="39dc4-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="39dc4-116">macOSCount</span></span>|<span data-ttu-id="39dc4-117">Int32</span><span class="sxs-lookup"><span data-stu-id="39dc4-117">Int32</span></span>|<span data-ttu-id="39dc4-118">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39dc4-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="39dc4-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="39dc4-119">windowsMobileCount</span></span>|<span data-ttu-id="39dc4-120">Int32</span><span class="sxs-lookup"><span data-stu-id="39dc4-120">Int32</span></span>|<span data-ttu-id="39dc4-121">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39dc4-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="39dc4-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="39dc4-122">windowsCount</span></span>|<span data-ttu-id="39dc4-123">Int32</span><span class="sxs-lookup"><span data-stu-id="39dc4-123">Int32</span></span>|<span data-ttu-id="39dc4-124">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39dc4-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="39dc4-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="39dc4-125">unknownCount</span></span>|<span data-ttu-id="39dc4-126">Int32</span><span class="sxs-lookup"><span data-stu-id="39dc4-126">Int32</span></span>|<span data-ttu-id="39dc4-127">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39dc4-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39dc4-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39dc4-128">Relationships</span></span>
<span data-ttu-id="39dc4-129">なし</span><span class="sxs-lookup"><span data-stu-id="39dc4-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39dc4-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39dc4-130">JSON Representation</span></span>
<span data-ttu-id="39dc4-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39dc4-131">Here is a JSON representation of the resource.</span></span>
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



