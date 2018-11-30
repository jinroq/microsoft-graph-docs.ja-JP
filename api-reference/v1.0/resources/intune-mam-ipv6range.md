---
title: iPv6Range リソースの種類
description: IP V6 の範囲
ms.openlocfilehash: c2f17529b589fc2d7837f6a8f539ff64d5d82dd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024229"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="2a3ac-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a3ac-103">iPv6Range resource type</span></span>

> <span data-ttu-id="2a3ac-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a3ac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a3ac-105">IP V6 の範囲</span><span class="sxs-lookup"><span data-stu-id="2a3ac-105">IP V6 range</span></span>

<span data-ttu-id="2a3ac-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2a3ac-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2a3ac-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a3ac-107">Properties</span></span>
|<span data-ttu-id="2a3ac-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a3ac-108">Property</span></span>|<span data-ttu-id="2a3ac-109">型</span><span class="sxs-lookup"><span data-stu-id="2a3ac-109">Type</span></span>|<span data-ttu-id="2a3ac-110">説明</span><span class="sxs-lookup"><span data-stu-id="2a3ac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a3ac-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="2a3ac-111">lowerAddress</span></span>|<span data-ttu-id="2a3ac-112">文字列</span><span class="sxs-lookup"><span data-stu-id="2a3ac-112">String</span></span>|<span data-ttu-id="2a3ac-113">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="2a3ac-113">Lower IP Address</span></span>|
|<span data-ttu-id="2a3ac-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="2a3ac-114">upperAddress</span></span>|<span data-ttu-id="2a3ac-115">文字列</span><span class="sxs-lookup"><span data-stu-id="2a3ac-115">String</span></span>|<span data-ttu-id="2a3ac-116">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="2a3ac-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a3ac-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a3ac-117">Relationships</span></span>
<span data-ttu-id="2a3ac-118">なし</span><span class="sxs-lookup"><span data-stu-id="2a3ac-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a3ac-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a3ac-119">JSON Representation</span></span>
<span data-ttu-id="2a3ac-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a3ac-120">Here is a JSON representation of the resource.</span></span>
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



