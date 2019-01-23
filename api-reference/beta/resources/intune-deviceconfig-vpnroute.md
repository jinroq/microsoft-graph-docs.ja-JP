---
title: vpnRoute リソースの種類
description: VPN 経路の定義です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 628e2f384b06dece13da1595a4111a2d1022a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423021"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="45339-103">vpnRoute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45339-103">vpnRoute resource type</span></span>

> <span data-ttu-id="45339-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="45339-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45339-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45339-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45339-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45339-107">VPN 経路の定義です。</span><span class="sxs-lookup"><span data-stu-id="45339-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="45339-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45339-108">Properties</span></span>
|<span data-ttu-id="45339-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45339-109">Property</span></span>|<span data-ttu-id="45339-110">型</span><span class="sxs-lookup"><span data-stu-id="45339-110">Type</span></span>|<span data-ttu-id="45339-111">説明</span><span class="sxs-lookup"><span data-stu-id="45339-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45339-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="45339-112">destinationPrefix</span></span>|<span data-ttu-id="45339-113">String</span><span class="sxs-lookup"><span data-stu-id="45339-113">String</span></span>|<span data-ttu-id="45339-114">宛先プレフィックス (IPv4 と v6 アドレス)。</span><span class="sxs-lookup"><span data-stu-id="45339-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="45339-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="45339-115">prefixSize</span></span>|<span data-ttu-id="45339-116">Int32</span><span class="sxs-lookup"><span data-stu-id="45339-116">Int32</span></span>|<span data-ttu-id="45339-117">プレフィックスのサイズです。</span><span class="sxs-lookup"><span data-stu-id="45339-117">Prefix size.</span></span> <span data-ttu-id="45339-118">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="45339-118">(1-32).</span></span> <span data-ttu-id="45339-119">有効な値 1 ~ 32</span><span class="sxs-lookup"><span data-stu-id="45339-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="45339-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="45339-120">Relationships</span></span>
<span data-ttu-id="45339-121">なし</span><span class="sxs-lookup"><span data-stu-id="45339-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45339-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45339-122">JSON Representation</span></span>
<span data-ttu-id="45339-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="45339-123">Here is a JSON representation of the resource.</span></span>
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




