---
title: vpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
author: tfitzmac
ms.openlocfilehash: f622d476e041fd89a639c14113e273a16aca992f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333475"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="04872-103">vpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04872-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="04872-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04872-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04872-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04872-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04872-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04872-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04872-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="04872-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="04872-108">Properties</span><span class="sxs-lookup"><span data-stu-id="04872-108">Properties</span></span>
|<span data-ttu-id="04872-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04872-109">Property</span></span>|<span data-ttu-id="04872-110">種類</span><span class="sxs-lookup"><span data-stu-id="04872-110">Type</span></span>|<span data-ttu-id="04872-111">説明</span><span class="sxs-lookup"><span data-stu-id="04872-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04872-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="04872-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="04872-113">String</span><span class="sxs-lookup"><span data-stu-id="04872-113">String</span></span>|<span data-ttu-id="04872-114">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="04872-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="04872-115">address</span><span class="sxs-lookup"><span data-stu-id="04872-115">address</span></span>|<span data-ttu-id="04872-116">String</span><span class="sxs-lookup"><span data-stu-id="04872-116">String</span></span>|<span data-ttu-id="04872-117">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="04872-117">Address.</span></span>|
|<span data-ttu-id="04872-118">port</span><span class="sxs-lookup"><span data-stu-id="04872-118">port</span></span>|<span data-ttu-id="04872-119">Int32</span><span class="sxs-lookup"><span data-stu-id="04872-119">Int32</span></span>|<span data-ttu-id="04872-120">ポートです。</span><span class="sxs-lookup"><span data-stu-id="04872-120">Port.</span></span> <span data-ttu-id="04872-121">0 から 65535 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="04872-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="04872-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="04872-122">Relationships</span></span>
<span data-ttu-id="04872-123">なし</span><span class="sxs-lookup"><span data-stu-id="04872-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04872-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04872-124">JSON Representation</span></span>
<span data-ttu-id="04872-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04872-125">Here is a JSON representation of the resource.</span></span>
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





