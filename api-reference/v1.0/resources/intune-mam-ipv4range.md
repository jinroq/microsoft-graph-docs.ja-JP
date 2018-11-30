---
title: iPv4Range リソースの種類
description: IP V4 範囲
ms.openlocfilehash: 8b59101e1fcdb5ab88d9c24a0359f8abb1687818
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023044"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="b54da-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b54da-103">iPv4Range resource type</span></span>

> <span data-ttu-id="b54da-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b54da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b54da-105">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="b54da-105">IP V4 range</span></span>

<span data-ttu-id="b54da-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b54da-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b54da-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b54da-107">Properties</span></span>
|<span data-ttu-id="b54da-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b54da-108">Property</span></span>|<span data-ttu-id="b54da-109">型</span><span class="sxs-lookup"><span data-stu-id="b54da-109">Type</span></span>|<span data-ttu-id="b54da-110">説明</span><span class="sxs-lookup"><span data-stu-id="b54da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b54da-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="b54da-111">lowerAddress</span></span>|<span data-ttu-id="b54da-112">文字列</span><span class="sxs-lookup"><span data-stu-id="b54da-112">String</span></span>|<span data-ttu-id="b54da-113">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="b54da-113">Lower IP Address</span></span>|
|<span data-ttu-id="b54da-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="b54da-114">upperAddress</span></span>|<span data-ttu-id="b54da-115">文字列</span><span class="sxs-lookup"><span data-stu-id="b54da-115">String</span></span>|<span data-ttu-id="b54da-116">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="b54da-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="b54da-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b54da-117">Relationships</span></span>
<span data-ttu-id="b54da-118">なし</span><span class="sxs-lookup"><span data-stu-id="b54da-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b54da-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b54da-119">JSON Representation</span></span>
<span data-ttu-id="b54da-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b54da-120">Here is a JSON representation of the resource.</span></span>
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



