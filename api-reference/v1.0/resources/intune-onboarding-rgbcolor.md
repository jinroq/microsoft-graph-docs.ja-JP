---
title: rgbColor リソースの種類
description: RGB 色。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fc40b5cc2ffff02bed89847386db6398f76b3953
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967008"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="8d129-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d129-103">rgbColor resource type</span></span>

> <span data-ttu-id="8d129-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8d129-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d129-105">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="8d129-105">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="8d129-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d129-106">Properties</span></span>
|<span data-ttu-id="8d129-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d129-107">Property</span></span>|<span data-ttu-id="8d129-108">種類</span><span class="sxs-lookup"><span data-stu-id="8d129-108">Type</span></span>|<span data-ttu-id="8d129-109">説明</span><span class="sxs-lookup"><span data-stu-id="8d129-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d129-110">r</span><span class="sxs-lookup"><span data-stu-id="8d129-110">r</span></span>|<span data-ttu-id="8d129-111">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="8d129-111">Byte</span></span>|<span data-ttu-id="8d129-112">赤の値</span><span class="sxs-lookup"><span data-stu-id="8d129-112">Red value</span></span>|
|<span data-ttu-id="8d129-113">g</span><span class="sxs-lookup"><span data-stu-id="8d129-113">g</span></span>|<span data-ttu-id="8d129-114">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="8d129-114">Byte</span></span>|<span data-ttu-id="8d129-115">緑の値</span><span class="sxs-lookup"><span data-stu-id="8d129-115">Green value</span></span>|
|<span data-ttu-id="8d129-116">b</span><span class="sxs-lookup"><span data-stu-id="8d129-116">b</span></span>|<span data-ttu-id="8d129-117">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="8d129-117">Byte</span></span>|<span data-ttu-id="8d129-118">青の値</span><span class="sxs-lookup"><span data-stu-id="8d129-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d129-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8d129-119">Relationships</span></span>
<span data-ttu-id="8d129-120">なし</span><span class="sxs-lookup"><span data-stu-id="8d129-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8d129-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d129-121">JSON Representation</span></span>
<span data-ttu-id="8d129-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8d129-122">Here is a JSON representation of the resource.</span></span>
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



