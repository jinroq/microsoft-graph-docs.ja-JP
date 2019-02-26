---
title: iPv6Range リソースの種類
description: IPv6 範囲の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f171a8ebb28d15e78a30bf542c37a163f0d097f0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258990"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="21406-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21406-103">iPv6Range resource type</span></span>

> <span data-ttu-id="21406-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="21406-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21406-105">IPv6 範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="21406-105">IPv6 Range definition.</span></span>


<span data-ttu-id="21406-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="21406-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21406-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21406-107">Properties</span></span>
|<span data-ttu-id="21406-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21406-108">Property</span></span>|<span data-ttu-id="21406-109">型</span><span class="sxs-lookup"><span data-stu-id="21406-109">Type</span></span>|<span data-ttu-id="21406-110">説明</span><span class="sxs-lookup"><span data-stu-id="21406-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21406-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="21406-111">lowerAddress</span></span>|<span data-ttu-id="21406-112">String</span><span class="sxs-lookup"><span data-stu-id="21406-112">String</span></span>|<span data-ttu-id="21406-113">下のアドレス</span><span class="sxs-lookup"><span data-stu-id="21406-113">Lower address</span></span>|
|<span data-ttu-id="21406-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="21406-114">upperAddress</span></span>|<span data-ttu-id="21406-115">文字列</span><span class="sxs-lookup"><span data-stu-id="21406-115">String</span></span>|<span data-ttu-id="21406-116">上住所</span><span class="sxs-lookup"><span data-stu-id="21406-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="21406-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21406-117">Relationships</span></span>
<span data-ttu-id="21406-118">なし</span><span class="sxs-lookup"><span data-stu-id="21406-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21406-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21406-119">JSON Representation</span></span>
<span data-ttu-id="21406-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21406-120">Here is a JSON representation of the resource.</span></span>
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



