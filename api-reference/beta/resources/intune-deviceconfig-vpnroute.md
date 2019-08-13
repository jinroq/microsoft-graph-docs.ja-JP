---
title: vpnRoute リソースの種類
description: VPN ルートの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00f5d1eb3f05d11833e687d002e1d698a366fd61
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367611"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="59700-103">vpnRoute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59700-103">vpnRoute resource type</span></span>

> <span data-ttu-id="59700-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59700-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59700-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="59700-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59700-106">VPN ルートの定義。</span><span class="sxs-lookup"><span data-stu-id="59700-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="59700-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59700-107">Properties</span></span>
|<span data-ttu-id="59700-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59700-108">Property</span></span>|<span data-ttu-id="59700-109">型</span><span class="sxs-lookup"><span data-stu-id="59700-109">Type</span></span>|<span data-ttu-id="59700-110">説明</span><span class="sxs-lookup"><span data-stu-id="59700-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59700-111">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="59700-111">destinationPrefix</span></span>|<span data-ttu-id="59700-112">String</span><span class="sxs-lookup"><span data-stu-id="59700-112">String</span></span>|<span data-ttu-id="59700-113">宛先プレフィックス (IPv4/v6 アドレス)。</span><span class="sxs-lookup"><span data-stu-id="59700-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="59700-114">prefixSize</span><span class="sxs-lookup"><span data-stu-id="59700-114">prefixSize</span></span>|<span data-ttu-id="59700-115">Int32</span><span class="sxs-lookup"><span data-stu-id="59700-115">Int32</span></span>|<span data-ttu-id="59700-116">プレフィックスのサイズです。</span><span class="sxs-lookup"><span data-stu-id="59700-116">Prefix size.</span></span> <span data-ttu-id="59700-117">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="59700-117">(1-32).</span></span> <span data-ttu-id="59700-118">有効な値は 1 ~ 32</span><span class="sxs-lookup"><span data-stu-id="59700-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="59700-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59700-119">Relationships</span></span>
<span data-ttu-id="59700-120">なし</span><span class="sxs-lookup"><span data-stu-id="59700-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59700-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59700-121">JSON Representation</span></span>
<span data-ttu-id="59700-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59700-122">Here is a JSON representation of the resource.</span></span>
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



