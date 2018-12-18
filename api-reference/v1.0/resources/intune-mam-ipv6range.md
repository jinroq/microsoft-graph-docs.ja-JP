---
title: iPv6Range リソースの種類
description: IP V6 の範囲
author: tfitzmac
ms.openlocfilehash: b5a2ad772d45b4be5fa3a8f4da04b28bc965195d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337549"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="8ec80-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ec80-103">iPv6Range resource type</span></span>

> <span data-ttu-id="8ec80-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ec80-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ec80-105">IP V6 の範囲</span><span class="sxs-lookup"><span data-stu-id="8ec80-105">IP V6 range</span></span>

<span data-ttu-id="8ec80-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8ec80-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ec80-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ec80-107">Properties</span></span>
|<span data-ttu-id="8ec80-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ec80-108">Property</span></span>|<span data-ttu-id="8ec80-109">種類</span><span class="sxs-lookup"><span data-stu-id="8ec80-109">Type</span></span>|<span data-ttu-id="8ec80-110">説明</span><span class="sxs-lookup"><span data-stu-id="8ec80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ec80-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="8ec80-111">lowerAddress</span></span>|<span data-ttu-id="8ec80-112">文字列</span><span class="sxs-lookup"><span data-stu-id="8ec80-112">String</span></span>|<span data-ttu-id="8ec80-113">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="8ec80-113">Lower IP Address</span></span>|
|<span data-ttu-id="8ec80-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="8ec80-114">upperAddress</span></span>|<span data-ttu-id="8ec80-115">文字列</span><span class="sxs-lookup"><span data-stu-id="8ec80-115">String</span></span>|<span data-ttu-id="8ec80-116">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="8ec80-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ec80-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8ec80-117">Relationships</span></span>
<span data-ttu-id="8ec80-118">なし</span><span class="sxs-lookup"><span data-stu-id="8ec80-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ec80-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ec80-119">JSON Representation</span></span>
<span data-ttu-id="8ec80-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8ec80-120">Here is a JSON representation of the resource.</span></span>
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



