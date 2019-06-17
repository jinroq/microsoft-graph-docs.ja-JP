---
title: iPv4Range リソースの種類
description: IPv4 の範囲定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c740cc94965ae41a857aa2c6ccb1394e161e6866
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996002"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="287ef-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="287ef-103">iPv4Range resource type</span></span>

> <span data-ttu-id="287ef-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="287ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="287ef-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="287ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="287ef-106">IPv4 の範囲定義。</span><span class="sxs-lookup"><span data-stu-id="287ef-106">IPv4 Range definition.</span></span>


<span data-ttu-id="287ef-107">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="287ef-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="287ef-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="287ef-108">Properties</span></span>
|<span data-ttu-id="287ef-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="287ef-109">Property</span></span>|<span data-ttu-id="287ef-110">型</span><span class="sxs-lookup"><span data-stu-id="287ef-110">Type</span></span>|<span data-ttu-id="287ef-111">説明</span><span class="sxs-lookup"><span data-stu-id="287ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="287ef-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="287ef-112">lowerAddress</span></span>|<span data-ttu-id="287ef-113">String</span><span class="sxs-lookup"><span data-stu-id="287ef-113">String</span></span>|<span data-ttu-id="287ef-114">小さいアドレス。</span><span class="sxs-lookup"><span data-stu-id="287ef-114">Lower address.</span></span>|
|<span data-ttu-id="287ef-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="287ef-115">upperAddress</span></span>|<span data-ttu-id="287ef-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="287ef-116">String</span></span>|<span data-ttu-id="287ef-117">上住所</span><span class="sxs-lookup"><span data-stu-id="287ef-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="287ef-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="287ef-118">Relationships</span></span>
<span data-ttu-id="287ef-119">なし</span><span class="sxs-lookup"><span data-stu-id="287ef-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="287ef-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="287ef-120">JSON Representation</span></span>
<span data-ttu-id="287ef-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="287ef-121">Here is a JSON representation of the resource.</span></span>
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





