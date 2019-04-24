---
title: iPv4Range リソースの種類
description: IPv4 の範囲定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14cb0d88013b13f57b186f5388d5ac89f60db043
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465525"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="ae8b6-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae8b6-103">iPv4Range resource type</span></span>

> <span data-ttu-id="ae8b6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae8b6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae8b6-105">IPv4 の範囲定義。</span><span class="sxs-lookup"><span data-stu-id="ae8b6-105">IPv4 Range definition.</span></span>


<span data-ttu-id="ae8b6-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ae8b6-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ae8b6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae8b6-107">Properties</span></span>
|<span data-ttu-id="ae8b6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae8b6-108">Property</span></span>|<span data-ttu-id="ae8b6-109">型</span><span class="sxs-lookup"><span data-stu-id="ae8b6-109">Type</span></span>|<span data-ttu-id="ae8b6-110">説明</span><span class="sxs-lookup"><span data-stu-id="ae8b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae8b6-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="ae8b6-111">lowerAddress</span></span>|<span data-ttu-id="ae8b6-112">String</span><span class="sxs-lookup"><span data-stu-id="ae8b6-112">String</span></span>|<span data-ttu-id="ae8b6-113">小さいアドレス。</span><span class="sxs-lookup"><span data-stu-id="ae8b6-113">Lower address.</span></span>|
|<span data-ttu-id="ae8b6-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="ae8b6-114">upperAddress</span></span>|<span data-ttu-id="ae8b6-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ae8b6-115">String</span></span>|<span data-ttu-id="ae8b6-116">上住所</span><span class="sxs-lookup"><span data-stu-id="ae8b6-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae8b6-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae8b6-117">Relationships</span></span>
<span data-ttu-id="ae8b6-118">なし</span><span class="sxs-lookup"><span data-stu-id="ae8b6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae8b6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae8b6-119">JSON Representation</span></span>
<span data-ttu-id="ae8b6-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae8b6-120">Here is a JSON representation of the resource.</span></span>
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



