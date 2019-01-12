---
title: vpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 727d26af7f2c1801cd06fc98949109efec267f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955353"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="206a4-103">vpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="206a4-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="206a4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="206a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="206a4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="206a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="206a4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="206a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="206a4-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="206a4-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="206a4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="206a4-108">Properties</span></span>
|<span data-ttu-id="206a4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="206a4-109">Property</span></span>|<span data-ttu-id="206a4-110">種類</span><span class="sxs-lookup"><span data-stu-id="206a4-110">Type</span></span>|<span data-ttu-id="206a4-111">説明</span><span class="sxs-lookup"><span data-stu-id="206a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="206a4-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="206a4-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="206a4-113">String</span><span class="sxs-lookup"><span data-stu-id="206a4-113">String</span></span>|<span data-ttu-id="206a4-114">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="206a4-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="206a4-115">address</span><span class="sxs-lookup"><span data-stu-id="206a4-115">address</span></span>|<span data-ttu-id="206a4-116">String</span><span class="sxs-lookup"><span data-stu-id="206a4-116">String</span></span>|<span data-ttu-id="206a4-117">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="206a4-117">Address.</span></span>|
|<span data-ttu-id="206a4-118">port</span><span class="sxs-lookup"><span data-stu-id="206a4-118">port</span></span>|<span data-ttu-id="206a4-119">Int32</span><span class="sxs-lookup"><span data-stu-id="206a4-119">Int32</span></span>|<span data-ttu-id="206a4-120">ポートです。</span><span class="sxs-lookup"><span data-stu-id="206a4-120">Port.</span></span> <span data-ttu-id="206a4-121">0 から 65535 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="206a4-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="206a4-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="206a4-122">Relationships</span></span>
<span data-ttu-id="206a4-123">なし</span><span class="sxs-lookup"><span data-stu-id="206a4-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="206a4-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="206a4-124">JSON Representation</span></span>
<span data-ttu-id="206a4-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="206a4-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```





