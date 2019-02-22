---
title: vpnroute リソースの種類
description: VPN ルートの定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54706d47267eef8fff6c465f24e4e9caa183ccc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154300"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="d645f-103">vpnroute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d645f-103">vpnRoute resource type</span></span>

> <span data-ttu-id="d645f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d645f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d645f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d645f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d645f-106">VPN ルートの定義。</span><span class="sxs-lookup"><span data-stu-id="d645f-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d645f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d645f-107">Properties</span></span>
|<span data-ttu-id="d645f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d645f-108">Property</span></span>|<span data-ttu-id="d645f-109">型</span><span class="sxs-lookup"><span data-stu-id="d645f-109">Type</span></span>|<span data-ttu-id="d645f-110">説明</span><span class="sxs-lookup"><span data-stu-id="d645f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d645f-111">destinationprefix</span><span class="sxs-lookup"><span data-stu-id="d645f-111">destinationPrefix</span></span>|<span data-ttu-id="d645f-112">String</span><span class="sxs-lookup"><span data-stu-id="d645f-112">String</span></span>|<span data-ttu-id="d645f-113">宛先プレフィックス (IPv4/v6 アドレス)。</span><span class="sxs-lookup"><span data-stu-id="d645f-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="d645f-114">prefixSize</span><span class="sxs-lookup"><span data-stu-id="d645f-114">prefixSize</span></span>|<span data-ttu-id="d645f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d645f-115">Int32</span></span>|<span data-ttu-id="d645f-116">プレフィックスのサイズです。</span><span class="sxs-lookup"><span data-stu-id="d645f-116">Prefix size.</span></span> <span data-ttu-id="d645f-117">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="d645f-117">(1-32).</span></span> <span data-ttu-id="d645f-118">有効な値は 1 ~ 32</span><span class="sxs-lookup"><span data-stu-id="d645f-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="d645f-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d645f-119">Relationships</span></span>
<span data-ttu-id="d645f-120">なし</span><span class="sxs-lookup"><span data-stu-id="d645f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d645f-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d645f-121">JSON Representation</span></span>
<span data-ttu-id="d645f-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d645f-122">Here is a JSON representation of the resource.</span></span>
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




