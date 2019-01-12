---
title: iPv4Range リソースの種類
description: IP V4 範囲
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c260796259ce6084add7eadb48192ea50c209c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931931"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="96b12-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96b12-103">iPv4Range resource type</span></span>

> <span data-ttu-id="96b12-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="96b12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96b12-105">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="96b12-105">IP V4 range</span></span>

<span data-ttu-id="96b12-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="96b12-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96b12-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96b12-107">Properties</span></span>
|<span data-ttu-id="96b12-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96b12-108">Property</span></span>|<span data-ttu-id="96b12-109">種類</span><span class="sxs-lookup"><span data-stu-id="96b12-109">Type</span></span>|<span data-ttu-id="96b12-110">説明</span><span class="sxs-lookup"><span data-stu-id="96b12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96b12-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="96b12-111">lowerAddress</span></span>|<span data-ttu-id="96b12-112">文字列</span><span class="sxs-lookup"><span data-stu-id="96b12-112">String</span></span>|<span data-ttu-id="96b12-113">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="96b12-113">Lower IP Address</span></span>|
|<span data-ttu-id="96b12-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="96b12-114">upperAddress</span></span>|<span data-ttu-id="96b12-115">文字列</span><span class="sxs-lookup"><span data-stu-id="96b12-115">String</span></span>|<span data-ttu-id="96b12-116">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="96b12-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="96b12-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96b12-117">Relationships</span></span>
<span data-ttu-id="96b12-118">なし</span><span class="sxs-lookup"><span data-stu-id="96b12-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96b12-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96b12-119">JSON Representation</span></span>
<span data-ttu-id="96b12-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96b12-120">Here is a JSON representation of the resource.</span></span>
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



