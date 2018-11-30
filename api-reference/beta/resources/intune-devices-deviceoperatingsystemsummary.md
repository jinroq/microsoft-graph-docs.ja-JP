---
title: deviceOperatingSystemSummary リソースの種類
description: デバイスのオペレーティング システムの概要。
ms.openlocfilehash: 13224e18f117f13a6f7c7090d1aa9cb2686350c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074248"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="cb5ac-103">deviceOperatingSystemSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb5ac-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="cb5ac-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb5ac-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb5ac-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb5ac-107">デバイスのオペレーティング システムの要約です。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-107">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="cb5ac-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb5ac-108">Properties</span></span>
|<span data-ttu-id="cb5ac-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb5ac-109">Property</span></span>|<span data-ttu-id="cb5ac-110">型</span><span class="sxs-lookup"><span data-stu-id="cb5ac-110">Type</span></span>|<span data-ttu-id="cb5ac-111">説明</span><span class="sxs-lookup"><span data-stu-id="cb5ac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb5ac-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="cb5ac-112">androidCount</span></span>|<span data-ttu-id="cb5ac-113">Int32</span><span class="sxs-lookup"><span data-stu-id="cb5ac-113">Int32</span></span>|<span data-ttu-id="cb5ac-114">Android デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-114">Number of android device count.</span></span>|
|<span data-ttu-id="cb5ac-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="cb5ac-115">iosCount</span></span>|<span data-ttu-id="cb5ac-116">Int32</span><span class="sxs-lookup"><span data-stu-id="cb5ac-116">Int32</span></span>|<span data-ttu-id="cb5ac-117">iOS デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="cb5ac-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="cb5ac-118">macOSCount</span></span>|<span data-ttu-id="cb5ac-119">Int32</span><span class="sxs-lookup"><span data-stu-id="cb5ac-119">Int32</span></span>|<span data-ttu-id="cb5ac-120">Mac OS X デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="cb5ac-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="cb5ac-121">windowsMobileCount</span></span>|<span data-ttu-id="cb5ac-122">Int32</span><span class="sxs-lookup"><span data-stu-id="cb5ac-122">Int32</span></span>|<span data-ttu-id="cb5ac-123">Windows Mobile デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="cb5ac-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="cb5ac-124">windowsCount</span></span>|<span data-ttu-id="cb5ac-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cb5ac-125">Int32</span></span>|<span data-ttu-id="cb5ac-126">Windows デバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="cb5ac-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="cb5ac-127">unknownCount</span></span>|<span data-ttu-id="cb5ac-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cb5ac-128">Int32</span></span>|<span data-ttu-id="cb5ac-129">不明なデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb5ac-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cb5ac-130">Relationships</span></span>
<span data-ttu-id="cb5ac-131">なし</span><span class="sxs-lookup"><span data-stu-id="cb5ac-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb5ac-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb5ac-132">JSON Representation</span></span>
<span data-ttu-id="cb5ac-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cb5ac-133">Here is a JSON representation of the resource.</span></span>
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





