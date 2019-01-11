---
title: iPv6Range リソースの種類
description: IP V6 の範囲
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84d925cc7885dab4b3e87dbd62060894e741f52c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845747"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="f1a13-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1a13-103">iPv6Range resource type</span></span>

> <span data-ttu-id="f1a13-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1a13-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1a13-105">IP V6 の範囲</span><span class="sxs-lookup"><span data-stu-id="f1a13-105">IP V6 range</span></span>

<span data-ttu-id="f1a13-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f1a13-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1a13-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1a13-107">Properties</span></span>
|<span data-ttu-id="f1a13-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1a13-108">Property</span></span>|<span data-ttu-id="f1a13-109">種類</span><span class="sxs-lookup"><span data-stu-id="f1a13-109">Type</span></span>|<span data-ttu-id="f1a13-110">説明</span><span class="sxs-lookup"><span data-stu-id="f1a13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a13-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="f1a13-111">lowerAddress</span></span>|<span data-ttu-id="f1a13-112">文字列</span><span class="sxs-lookup"><span data-stu-id="f1a13-112">String</span></span>|<span data-ttu-id="f1a13-113">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="f1a13-113">Lower IP Address</span></span>|
|<span data-ttu-id="f1a13-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="f1a13-114">upperAddress</span></span>|<span data-ttu-id="f1a13-115">文字列</span><span class="sxs-lookup"><span data-stu-id="f1a13-115">String</span></span>|<span data-ttu-id="f1a13-116">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="f1a13-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1a13-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1a13-117">Relationships</span></span>
<span data-ttu-id="f1a13-118">なし</span><span class="sxs-lookup"><span data-stu-id="f1a13-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1a13-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1a13-119">JSON Representation</span></span>
<span data-ttu-id="f1a13-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1a13-120">Here is a JSON representation of the resource.</span></span>
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



