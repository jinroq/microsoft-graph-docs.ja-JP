---
title: iPv6Range リソースの種類
description: IP V6 の範囲
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 115c89b6ae90a292e08e7b0374e1c3b529e2df19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926863"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="33987-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="33987-103">iPv6Range resource type</span></span>

> <span data-ttu-id="33987-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="33987-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33987-105">IP V6 の範囲</span><span class="sxs-lookup"><span data-stu-id="33987-105">IP V6 range</span></span>

<span data-ttu-id="33987-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="33987-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33987-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33987-107">Properties</span></span>
|<span data-ttu-id="33987-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33987-108">Property</span></span>|<span data-ttu-id="33987-109">種類</span><span class="sxs-lookup"><span data-stu-id="33987-109">Type</span></span>|<span data-ttu-id="33987-110">説明</span><span class="sxs-lookup"><span data-stu-id="33987-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33987-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="33987-111">lowerAddress</span></span>|<span data-ttu-id="33987-112">文字列</span><span class="sxs-lookup"><span data-stu-id="33987-112">String</span></span>|<span data-ttu-id="33987-113">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="33987-113">Lower IP Address</span></span>|
|<span data-ttu-id="33987-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="33987-114">upperAddress</span></span>|<span data-ttu-id="33987-115">文字列</span><span class="sxs-lookup"><span data-stu-id="33987-115">String</span></span>|<span data-ttu-id="33987-116">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="33987-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="33987-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="33987-117">Relationships</span></span>
<span data-ttu-id="33987-118">なし</span><span class="sxs-lookup"><span data-stu-id="33987-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="33987-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="33987-119">JSON Representation</span></span>
<span data-ttu-id="33987-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="33987-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



