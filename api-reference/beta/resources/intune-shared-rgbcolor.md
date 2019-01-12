---
title: rgbColor リソースの種類
description: RGB 色。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3593c743d0b65d761abf18b7fdb4783d126c19f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928858"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="69d5c-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69d5c-103">rgbColor resource type</span></span>

> <span data-ttu-id="69d5c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="69d5c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69d5c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69d5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69d5c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="69d5c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69d5c-107">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="69d5c-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="69d5c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69d5c-108">Properties</span></span>
|<span data-ttu-id="69d5c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69d5c-109">Property</span></span>|<span data-ttu-id="69d5c-110">種類</span><span class="sxs-lookup"><span data-stu-id="69d5c-110">Type</span></span>|<span data-ttu-id="69d5c-111">説明</span><span class="sxs-lookup"><span data-stu-id="69d5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69d5c-112">r</span><span class="sxs-lookup"><span data-stu-id="69d5c-112">r</span></span>|<span data-ttu-id="69d5c-113">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="69d5c-113">Byte</span></span>|<span data-ttu-id="69d5c-114">赤の値</span><span class="sxs-lookup"><span data-stu-id="69d5c-114">Red value</span></span>|
|<span data-ttu-id="69d5c-115">g</span><span class="sxs-lookup"><span data-stu-id="69d5c-115">g</span></span>|<span data-ttu-id="69d5c-116">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="69d5c-116">Byte</span></span>|<span data-ttu-id="69d5c-117">緑の値</span><span class="sxs-lookup"><span data-stu-id="69d5c-117">Green value</span></span>|
|<span data-ttu-id="69d5c-118">b</span><span class="sxs-lookup"><span data-stu-id="69d5c-118">b</span></span>|<span data-ttu-id="69d5c-119">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="69d5c-119">Byte</span></span>|<span data-ttu-id="69d5c-120">青の値</span><span class="sxs-lookup"><span data-stu-id="69d5c-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="69d5c-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="69d5c-121">Relationships</span></span>
<span data-ttu-id="69d5c-122">なし</span><span class="sxs-lookup"><span data-stu-id="69d5c-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="69d5c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69d5c-123">JSON Representation</span></span>
<span data-ttu-id="69d5c-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="69d5c-124">Here is a JSON representation of the resource.</span></span>
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





