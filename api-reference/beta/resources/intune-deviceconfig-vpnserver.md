---
title: vpnServer のリソースの種類
description: VPN サーバーの定義です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b48daa95cc2227f6d1691902a75614446c93a10a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889874"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="ae772-103">vpnServer のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae772-103">vpnServer resource type</span></span>

> <span data-ttu-id="ae772-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae772-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae772-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae772-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae772-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae772-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae772-107">VPN サーバーの定義です。</span><span class="sxs-lookup"><span data-stu-id="ae772-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="ae772-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae772-108">Properties</span></span>
|<span data-ttu-id="ae772-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae772-109">Property</span></span>|<span data-ttu-id="ae772-110">種類</span><span class="sxs-lookup"><span data-stu-id="ae772-110">Type</span></span>|<span data-ttu-id="ae772-111">説明</span><span class="sxs-lookup"><span data-stu-id="ae772-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae772-112">説明</span><span class="sxs-lookup"><span data-stu-id="ae772-112">description</span></span>|<span data-ttu-id="ae772-113">String</span><span class="sxs-lookup"><span data-stu-id="ae772-113">String</span></span>|<span data-ttu-id="ae772-114">説明。</span><span class="sxs-lookup"><span data-stu-id="ae772-114">Description.</span></span>|
|<span data-ttu-id="ae772-115">address</span><span class="sxs-lookup"><span data-stu-id="ae772-115">address</span></span>|<span data-ttu-id="ae772-116">String</span><span class="sxs-lookup"><span data-stu-id="ae772-116">String</span></span>|<span data-ttu-id="ae772-117">アドレス (IP アドレス、FQDN、または URL)</span><span class="sxs-lookup"><span data-stu-id="ae772-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="ae772-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="ae772-118">isDefaultServer</span></span>|<span data-ttu-id="ae772-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="ae772-119">Boolean</span></span>|<span data-ttu-id="ae772-120">既定のサーバーです。</span><span class="sxs-lookup"><span data-stu-id="ae772-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae772-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae772-121">Relationships</span></span>
<span data-ttu-id="ae772-122">なし</span><span class="sxs-lookup"><span data-stu-id="ae772-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ae772-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae772-123">JSON Representation</span></span>
<span data-ttu-id="ae772-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae772-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```





