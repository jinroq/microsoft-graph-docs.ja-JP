---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b4b53d7c7260e58458995093bbea17df5464e704
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846076"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="bc316-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc316-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="bc316-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bc316-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc316-105">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="bc316-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="bc316-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc316-106">Properties</span></span>
|<span data-ttu-id="bc316-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc316-107">Property</span></span>|<span data-ttu-id="bc316-108">種類</span><span class="sxs-lookup"><span data-stu-id="bc316-108">Type</span></span>|<span data-ttu-id="bc316-109">説明</span><span class="sxs-lookup"><span data-stu-id="bc316-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc316-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="bc316-110">androidCount</span></span>|<span data-ttu-id="bc316-111">Int32</span><span class="sxs-lookup"><span data-stu-id="bc316-111">Int32</span></span>|<span data-ttu-id="bc316-112">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="bc316-112">Number of android device count.</span></span>|
|<span data-ttu-id="bc316-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="bc316-113">iosCount</span></span>|<span data-ttu-id="bc316-114">Int32</span><span class="sxs-lookup"><span data-stu-id="bc316-114">Int32</span></span>|<span data-ttu-id="bc316-115">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="bc316-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="bc316-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="bc316-116">macOSCount</span></span>|<span data-ttu-id="bc316-117">Int32</span><span class="sxs-lookup"><span data-stu-id="bc316-117">Int32</span></span>|<span data-ttu-id="bc316-118">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="bc316-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="bc316-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="bc316-119">windowsMobileCount</span></span>|<span data-ttu-id="bc316-120">Int32</span><span class="sxs-lookup"><span data-stu-id="bc316-120">Int32</span></span>|<span data-ttu-id="bc316-121">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="bc316-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="bc316-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="bc316-122">windowsCount</span></span>|<span data-ttu-id="bc316-123">Int32</span><span class="sxs-lookup"><span data-stu-id="bc316-123">Int32</span></span>|<span data-ttu-id="bc316-124">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="bc316-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="bc316-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="bc316-125">unknownCount</span></span>|<span data-ttu-id="bc316-126">Int32</span><span class="sxs-lookup"><span data-stu-id="bc316-126">Int32</span></span>|<span data-ttu-id="bc316-127">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="bc316-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc316-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc316-128">Relationships</span></span>
<span data-ttu-id="bc316-129">なし</span><span class="sxs-lookup"><span data-stu-id="bc316-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc316-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc316-130">JSON Representation</span></span>
<span data-ttu-id="bc316-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc316-131">Here is a JSON representation of the resource.</span></span>
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



