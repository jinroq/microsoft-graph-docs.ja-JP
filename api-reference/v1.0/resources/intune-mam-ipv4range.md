---
title: iPv4Range リソースの種類
description: IP V4 範囲
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 593fc2287e888b38eadd3c588aaeeb51b31ea78f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816262"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="b37af-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b37af-103">iPv4Range resource type</span></span>

> <span data-ttu-id="b37af-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b37af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b37af-105">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="b37af-105">IP V4 range</span></span>

<span data-ttu-id="b37af-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b37af-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b37af-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b37af-107">Properties</span></span>
|<span data-ttu-id="b37af-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b37af-108">Property</span></span>|<span data-ttu-id="b37af-109">種類</span><span class="sxs-lookup"><span data-stu-id="b37af-109">Type</span></span>|<span data-ttu-id="b37af-110">説明</span><span class="sxs-lookup"><span data-stu-id="b37af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b37af-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="b37af-111">lowerAddress</span></span>|<span data-ttu-id="b37af-112">文字列</span><span class="sxs-lookup"><span data-stu-id="b37af-112">String</span></span>|<span data-ttu-id="b37af-113">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="b37af-113">Lower IP Address</span></span>|
|<span data-ttu-id="b37af-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="b37af-114">upperAddress</span></span>|<span data-ttu-id="b37af-115">文字列</span><span class="sxs-lookup"><span data-stu-id="b37af-115">String</span></span>|<span data-ttu-id="b37af-116">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="b37af-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="b37af-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b37af-117">Relationships</span></span>
<span data-ttu-id="b37af-118">なし</span><span class="sxs-lookup"><span data-stu-id="b37af-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b37af-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b37af-119">JSON Representation</span></span>
<span data-ttu-id="b37af-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b37af-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



