---
title: vpnroute リソースの種類
description: VPN ルートの定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c13cb40b5324620eebeb7230135ef981dba84f36
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807715"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="3a64b-103">vpnroute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a64b-103">vpnRoute resource type</span></span>

> <span data-ttu-id="3a64b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a64b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a64b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a64b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a64b-106">VPN ルートの定義。</span><span class="sxs-lookup"><span data-stu-id="3a64b-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3a64b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a64b-107">Properties</span></span>
|<span data-ttu-id="3a64b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a64b-108">Property</span></span>|<span data-ttu-id="3a64b-109">型</span><span class="sxs-lookup"><span data-stu-id="3a64b-109">Type</span></span>|<span data-ttu-id="3a64b-110">説明</span><span class="sxs-lookup"><span data-stu-id="3a64b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a64b-111">destinationprefix</span><span class="sxs-lookup"><span data-stu-id="3a64b-111">destinationPrefix</span></span>|<span data-ttu-id="3a64b-112">文字列</span><span class="sxs-lookup"><span data-stu-id="3a64b-112">String</span></span>|<span data-ttu-id="3a64b-113">宛先プレフィックス (IPv4/v6 アドレス)。</span><span class="sxs-lookup"><span data-stu-id="3a64b-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="3a64b-114">prefixSize</span><span class="sxs-lookup"><span data-stu-id="3a64b-114">prefixSize</span></span>|<span data-ttu-id="3a64b-115">Int32</span><span class="sxs-lookup"><span data-stu-id="3a64b-115">Int32</span></span>|<span data-ttu-id="3a64b-116">プレフィックスのサイズです。</span><span class="sxs-lookup"><span data-stu-id="3a64b-116">Prefix size.</span></span> <span data-ttu-id="3a64b-117">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="3a64b-117">(1-32).</span></span> <span data-ttu-id="3a64b-118">有効な値は 1 ~ 32</span><span class="sxs-lookup"><span data-stu-id="3a64b-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a64b-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a64b-119">Relationships</span></span>
<span data-ttu-id="3a64b-120">なし</span><span class="sxs-lookup"><span data-stu-id="3a64b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a64b-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a64b-121">JSON Representation</span></span>
<span data-ttu-id="3a64b-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a64b-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```





