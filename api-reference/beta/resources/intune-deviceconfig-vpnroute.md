---
title: vpnRoute リソースの種類
description: VPN 経路の定義です。
ms.openlocfilehash: 385ed5f369660805afa8cf935273b6689fc90173
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071780"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="8af00-103">vpnRoute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8af00-103">vpnRoute resource type</span></span>

> <span data-ttu-id="8af00-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8af00-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8af00-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8af00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8af00-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8af00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8af00-107">VPN 経路の定義です。</span><span class="sxs-lookup"><span data-stu-id="8af00-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="8af00-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8af00-108">Properties</span></span>
|<span data-ttu-id="8af00-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8af00-109">Property</span></span>|<span data-ttu-id="8af00-110">型</span><span class="sxs-lookup"><span data-stu-id="8af00-110">Type</span></span>|<span data-ttu-id="8af00-111">説明</span><span class="sxs-lookup"><span data-stu-id="8af00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8af00-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="8af00-112">destinationPrefix</span></span>|<span data-ttu-id="8af00-113">String</span><span class="sxs-lookup"><span data-stu-id="8af00-113">String</span></span>|<span data-ttu-id="8af00-114">宛先プレフィックス (IPv4 と v6 アドレス)。</span><span class="sxs-lookup"><span data-stu-id="8af00-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="8af00-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="8af00-115">prefixSize</span></span>|<span data-ttu-id="8af00-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8af00-116">Int32</span></span>|<span data-ttu-id="8af00-117">プレフィックスのサイズです。</span><span class="sxs-lookup"><span data-stu-id="8af00-117">Prefix size.</span></span> <span data-ttu-id="8af00-118">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="8af00-118">(1-32).</span></span> <span data-ttu-id="8af00-119">有効な値 1 ~ 32</span><span class="sxs-lookup"><span data-stu-id="8af00-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="8af00-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8af00-120">Relationships</span></span>
<span data-ttu-id="8af00-121">なし</span><span class="sxs-lookup"><span data-stu-id="8af00-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8af00-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8af00-122">JSON Representation</span></span>
<span data-ttu-id="8af00-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8af00-123">Here is a JSON representation of the resource.</span></span>
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





