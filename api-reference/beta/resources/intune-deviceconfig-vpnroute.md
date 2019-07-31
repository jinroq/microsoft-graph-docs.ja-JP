---
title: vpnRoute リソースの種類
description: VPN ルートの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c12e39a3f26fe5a25d0dca522e8d2ab3e774957
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969437"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="06a46-103">vpnRoute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06a46-103">vpnRoute resource type</span></span>

> <span data-ttu-id="06a46-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06a46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06a46-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06a46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06a46-106">VPN ルートの定義。</span><span class="sxs-lookup"><span data-stu-id="06a46-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="06a46-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06a46-107">Properties</span></span>
|<span data-ttu-id="06a46-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06a46-108">Property</span></span>|<span data-ttu-id="06a46-109">型</span><span class="sxs-lookup"><span data-stu-id="06a46-109">Type</span></span>|<span data-ttu-id="06a46-110">説明</span><span class="sxs-lookup"><span data-stu-id="06a46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06a46-111">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="06a46-111">destinationPrefix</span></span>|<span data-ttu-id="06a46-112">String</span><span class="sxs-lookup"><span data-stu-id="06a46-112">String</span></span>|<span data-ttu-id="06a46-113">宛先プレフィックス (IPv4/v6 アドレス)。</span><span class="sxs-lookup"><span data-stu-id="06a46-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="06a46-114">prefixSize</span><span class="sxs-lookup"><span data-stu-id="06a46-114">prefixSize</span></span>|<span data-ttu-id="06a46-115">Int32</span><span class="sxs-lookup"><span data-stu-id="06a46-115">Int32</span></span>|<span data-ttu-id="06a46-116">プレフィックスのサイズです。</span><span class="sxs-lookup"><span data-stu-id="06a46-116">Prefix size.</span></span> <span data-ttu-id="06a46-117">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="06a46-117">(1-32).</span></span> <span data-ttu-id="06a46-118">有効な値は 1 ~ 32</span><span class="sxs-lookup"><span data-stu-id="06a46-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="06a46-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06a46-119">Relationships</span></span>
<span data-ttu-id="06a46-120">なし</span><span class="sxs-lookup"><span data-stu-id="06a46-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06a46-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06a46-121">JSON Representation</span></span>
<span data-ttu-id="06a46-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06a46-122">Here is a JSON representation of the resource.</span></span>
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





