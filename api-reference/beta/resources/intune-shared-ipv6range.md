---
title: iPv6Range リソースの種類
description: IPv6 範囲の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51815dffc0048ec88b81cbe6034a42e108e5b222
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803571"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="82d3f-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82d3f-103">iPv6Range resource type</span></span>

> <span data-ttu-id="82d3f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82d3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82d3f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82d3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d3f-106">IPv6 範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="82d3f-106">IPv6 Range definition.</span></span>


<span data-ttu-id="82d3f-107">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="82d3f-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82d3f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82d3f-108">Properties</span></span>
|<span data-ttu-id="82d3f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82d3f-109">Property</span></span>|<span data-ttu-id="82d3f-110">型</span><span class="sxs-lookup"><span data-stu-id="82d3f-110">Type</span></span>|<span data-ttu-id="82d3f-111">説明</span><span class="sxs-lookup"><span data-stu-id="82d3f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d3f-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="82d3f-112">lowerAddress</span></span>|<span data-ttu-id="82d3f-113">文字列</span><span class="sxs-lookup"><span data-stu-id="82d3f-113">String</span></span>|<span data-ttu-id="82d3f-114">小さいアドレス。</span><span class="sxs-lookup"><span data-stu-id="82d3f-114">Lower address.</span></span>|
|<span data-ttu-id="82d3f-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="82d3f-115">upperAddress</span></span>|<span data-ttu-id="82d3f-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="82d3f-116">String</span></span>|<span data-ttu-id="82d3f-117">上住所</span><span class="sxs-lookup"><span data-stu-id="82d3f-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82d3f-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82d3f-118">Relationships</span></span>
<span data-ttu-id="82d3f-119">なし</span><span class="sxs-lookup"><span data-stu-id="82d3f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82d3f-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82d3f-120">JSON Representation</span></span>
<span data-ttu-id="82d3f-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82d3f-121">Here is a JSON representation of the resource.</span></span>
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





