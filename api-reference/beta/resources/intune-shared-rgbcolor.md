---
title: rgbColor リソースの種類
description: RGB 色。
ms.openlocfilehash: 7b5d450c0126e043a78a6c4f9f0e2fe6f06c7c13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072294"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="fbab5-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbab5-103">rgbColor resource type</span></span>

> <span data-ttu-id="fbab5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fbab5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbab5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbab5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbab5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fbab5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbab5-107">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="fbab5-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="fbab5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbab5-108">Properties</span></span>
|<span data-ttu-id="fbab5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbab5-109">Property</span></span>|<span data-ttu-id="fbab5-110">型</span><span class="sxs-lookup"><span data-stu-id="fbab5-110">Type</span></span>|<span data-ttu-id="fbab5-111">説明</span><span class="sxs-lookup"><span data-stu-id="fbab5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbab5-112">r</span><span class="sxs-lookup"><span data-stu-id="fbab5-112">r</span></span>|<span data-ttu-id="fbab5-113">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="fbab5-113">Byte</span></span>|<span data-ttu-id="fbab5-114">赤の値</span><span class="sxs-lookup"><span data-stu-id="fbab5-114">Red value</span></span>|
|<span data-ttu-id="fbab5-115">g</span><span class="sxs-lookup"><span data-stu-id="fbab5-115">g</span></span>|<span data-ttu-id="fbab5-116">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="fbab5-116">Byte</span></span>|<span data-ttu-id="fbab5-117">緑の値</span><span class="sxs-lookup"><span data-stu-id="fbab5-117">Green value</span></span>|
|<span data-ttu-id="fbab5-118">b</span><span class="sxs-lookup"><span data-stu-id="fbab5-118">b</span></span>|<span data-ttu-id="fbab5-119">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="fbab5-119">Byte</span></span>|<span data-ttu-id="fbab5-120">青の値</span><span class="sxs-lookup"><span data-stu-id="fbab5-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbab5-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbab5-121">Relationships</span></span>
<span data-ttu-id="fbab5-122">なし</span><span class="sxs-lookup"><span data-stu-id="fbab5-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbab5-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbab5-123">JSON Representation</span></span>
<span data-ttu-id="fbab5-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fbab5-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```





