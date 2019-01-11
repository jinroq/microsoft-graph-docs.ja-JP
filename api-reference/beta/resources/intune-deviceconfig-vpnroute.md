---
title: vpnRoute リソースの種類
description: VPN 経路の定義です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eaa74a1cef7d2eee8148e240cd80ca72f94adcb4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860572"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="016c7-103">vpnRoute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="016c7-103">vpnRoute resource type</span></span>

> <span data-ttu-id="016c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="016c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="016c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="016c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="016c7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="016c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="016c7-107">VPN 経路の定義です。</span><span class="sxs-lookup"><span data-stu-id="016c7-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="016c7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="016c7-108">Properties</span></span>
|<span data-ttu-id="016c7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="016c7-109">Property</span></span>|<span data-ttu-id="016c7-110">種類</span><span class="sxs-lookup"><span data-stu-id="016c7-110">Type</span></span>|<span data-ttu-id="016c7-111">説明</span><span class="sxs-lookup"><span data-stu-id="016c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="016c7-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="016c7-112">destinationPrefix</span></span>|<span data-ttu-id="016c7-113">String</span><span class="sxs-lookup"><span data-stu-id="016c7-113">String</span></span>|<span data-ttu-id="016c7-114">宛先プレフィックス (IPv4 と v6 アドレス)。</span><span class="sxs-lookup"><span data-stu-id="016c7-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="016c7-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="016c7-115">prefixSize</span></span>|<span data-ttu-id="016c7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="016c7-116">Int32</span></span>|<span data-ttu-id="016c7-117">プレフィックスのサイズです。</span><span class="sxs-lookup"><span data-stu-id="016c7-117">Prefix size.</span></span> <span data-ttu-id="016c7-118">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="016c7-118">(1-32).</span></span> <span data-ttu-id="016c7-119">有効な値 1 ~ 32</span><span class="sxs-lookup"><span data-stu-id="016c7-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="016c7-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="016c7-120">Relationships</span></span>
<span data-ttu-id="016c7-121">なし</span><span class="sxs-lookup"><span data-stu-id="016c7-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="016c7-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="016c7-122">JSON Representation</span></span>
<span data-ttu-id="016c7-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="016c7-123">Here is a JSON representation of the resource.</span></span>
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





