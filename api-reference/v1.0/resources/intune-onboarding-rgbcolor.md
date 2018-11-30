---
title: rgbColor リソースの種類
description: RGB 色。
ms.openlocfilehash: 5b3ef1f7b26925721098f82ec2bf54c614ce399b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024168"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="4ef47-103">rgbColor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ef47-103">rgbColor resource type</span></span>

> <span data-ttu-id="4ef47-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ef47-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ef47-105">RGB 色。</span><span class="sxs-lookup"><span data-stu-id="4ef47-105">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="4ef47-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ef47-106">Properties</span></span>
|<span data-ttu-id="4ef47-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ef47-107">Property</span></span>|<span data-ttu-id="4ef47-108">型</span><span class="sxs-lookup"><span data-stu-id="4ef47-108">Type</span></span>|<span data-ttu-id="4ef47-109">説明</span><span class="sxs-lookup"><span data-stu-id="4ef47-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ef47-110">r</span><span class="sxs-lookup"><span data-stu-id="4ef47-110">r</span></span>|<span data-ttu-id="4ef47-111">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="4ef47-111">Byte</span></span>|<span data-ttu-id="4ef47-112">赤の値</span><span class="sxs-lookup"><span data-stu-id="4ef47-112">Red value</span></span>|
|<span data-ttu-id="4ef47-113">g</span><span class="sxs-lookup"><span data-stu-id="4ef47-113">g</span></span>|<span data-ttu-id="4ef47-114">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="4ef47-114">Byte</span></span>|<span data-ttu-id="4ef47-115">緑の値</span><span class="sxs-lookup"><span data-stu-id="4ef47-115">Green value</span></span>|
|<span data-ttu-id="4ef47-116">b</span><span class="sxs-lookup"><span data-stu-id="4ef47-116">b</span></span>|<span data-ttu-id="4ef47-117">バイト型 (Byte)</span><span class="sxs-lookup"><span data-stu-id="4ef47-117">Byte</span></span>|<span data-ttu-id="4ef47-118">青の値</span><span class="sxs-lookup"><span data-stu-id="4ef47-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ef47-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ef47-119">Relationships</span></span>
<span data-ttu-id="4ef47-120">なし</span><span class="sxs-lookup"><span data-stu-id="4ef47-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4ef47-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ef47-121">JSON Representation</span></span>
<span data-ttu-id="4ef47-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4ef47-122">Here is a JSON representation of the resource.</span></span>
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



