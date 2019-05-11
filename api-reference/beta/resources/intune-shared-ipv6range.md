---
title: iPv6Range リソースの種類
description: IPv6 範囲の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b767b5af514045c52dec57244d186d7ff3feb9f8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940562"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="65256-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65256-103">iPv6Range resource type</span></span>

> <span data-ttu-id="65256-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65256-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65256-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65256-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65256-106">IPv6 範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="65256-106">IPv6 Range definition.</span></span>


<span data-ttu-id="65256-107">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="65256-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65256-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65256-108">Properties</span></span>
|<span data-ttu-id="65256-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65256-109">Property</span></span>|<span data-ttu-id="65256-110">型</span><span class="sxs-lookup"><span data-stu-id="65256-110">Type</span></span>|<span data-ttu-id="65256-111">説明</span><span class="sxs-lookup"><span data-stu-id="65256-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65256-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="65256-112">lowerAddress</span></span>|<span data-ttu-id="65256-113">String</span><span class="sxs-lookup"><span data-stu-id="65256-113">String</span></span>|<span data-ttu-id="65256-114">小さいアドレス。</span><span class="sxs-lookup"><span data-stu-id="65256-114">Lower address.</span></span>|
|<span data-ttu-id="65256-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="65256-115">upperAddress</span></span>|<span data-ttu-id="65256-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="65256-116">String</span></span>|<span data-ttu-id="65256-117">上住所</span><span class="sxs-lookup"><span data-stu-id="65256-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65256-118">関係</span><span class="sxs-lookup"><span data-stu-id="65256-118">Relationships</span></span>
<span data-ttu-id="65256-119">なし</span><span class="sxs-lookup"><span data-stu-id="65256-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65256-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65256-120">JSON Representation</span></span>
<span data-ttu-id="65256-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65256-121">Here is a JSON representation of the resource.</span></span>
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




