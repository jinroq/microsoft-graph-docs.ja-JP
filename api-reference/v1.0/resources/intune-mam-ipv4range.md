---
title: iPv4Range リソースの種類
description: IPv4 の範囲定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40845b43a50391613e23bf1c4885c382385b4f5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038138"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="966d4-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="966d4-103">iPv4Range resource type</span></span>

> <span data-ttu-id="966d4-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="966d4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="966d4-105">IPv4 の範囲定義。</span><span class="sxs-lookup"><span data-stu-id="966d4-105">IPv4 Range definition.</span></span>


<span data-ttu-id="966d4-106">[ipRange](../resources/intune-mam-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="966d4-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="966d4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="966d4-107">Properties</span></span>
|<span data-ttu-id="966d4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="966d4-108">Property</span></span>|<span data-ttu-id="966d4-109">型</span><span class="sxs-lookup"><span data-stu-id="966d4-109">Type</span></span>|<span data-ttu-id="966d4-110">説明</span><span class="sxs-lookup"><span data-stu-id="966d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="966d4-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="966d4-111">lowerAddress</span></span>|<span data-ttu-id="966d4-112">String</span><span class="sxs-lookup"><span data-stu-id="966d4-112">String</span></span>|<span data-ttu-id="966d4-113">小さいアドレス。</span><span class="sxs-lookup"><span data-stu-id="966d4-113">Lower address.</span></span>|
|<span data-ttu-id="966d4-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="966d4-114">upperAddress</span></span>|<span data-ttu-id="966d4-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="966d4-115">String</span></span>|<span data-ttu-id="966d4-116">上住所</span><span class="sxs-lookup"><span data-stu-id="966d4-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="966d4-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="966d4-117">Relationships</span></span>
<span data-ttu-id="966d4-118">なし</span><span class="sxs-lookup"><span data-stu-id="966d4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="966d4-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="966d4-119">JSON Representation</span></span>
<span data-ttu-id="966d4-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="966d4-120">Here is a JSON representation of the resource.</span></span>
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



