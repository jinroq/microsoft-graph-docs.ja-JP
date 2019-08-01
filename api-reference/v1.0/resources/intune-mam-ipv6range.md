---
title: iPv6Range リソースの種類
description: IPv6 範囲の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04183f443d767236a1a7c0afb1d1ed9b92c37889
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038144"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="2b0cb-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b0cb-103">iPv6Range resource type</span></span>

> <span data-ttu-id="2b0cb-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2b0cb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b0cb-105">IPv6 範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="2b0cb-105">IPv6 Range definition.</span></span>


<span data-ttu-id="2b0cb-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2b0cb-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2b0cb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b0cb-107">Properties</span></span>
|<span data-ttu-id="2b0cb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b0cb-108">Property</span></span>|<span data-ttu-id="2b0cb-109">型</span><span class="sxs-lookup"><span data-stu-id="2b0cb-109">Type</span></span>|<span data-ttu-id="2b0cb-110">説明</span><span class="sxs-lookup"><span data-stu-id="2b0cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b0cb-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="2b0cb-111">lowerAddress</span></span>|<span data-ttu-id="2b0cb-112">String</span><span class="sxs-lookup"><span data-stu-id="2b0cb-112">String</span></span>|<span data-ttu-id="2b0cb-113">下のアドレス</span><span class="sxs-lookup"><span data-stu-id="2b0cb-113">Lower address</span></span>|
|<span data-ttu-id="2b0cb-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="2b0cb-114">upperAddress</span></span>|<span data-ttu-id="2b0cb-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2b0cb-115">String</span></span>|<span data-ttu-id="2b0cb-116">上住所</span><span class="sxs-lookup"><span data-stu-id="2b0cb-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b0cb-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b0cb-117">Relationships</span></span>
<span data-ttu-id="2b0cb-118">なし</span><span class="sxs-lookup"><span data-stu-id="2b0cb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b0cb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b0cb-119">JSON Representation</span></span>
<span data-ttu-id="2b0cb-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b0cb-120">Here is a JSON representation of the resource.</span></span>
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



