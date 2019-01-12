---
title: windows10VpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4b34d105900478a1bcbc811e782e1ceaf94f251
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912275"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="51b26-103">windows10VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51b26-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="51b26-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51b26-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51b26-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51b26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51b26-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51b26-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51b26-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="51b26-107">VPN Proxy Server.</span></span>

<span data-ttu-id="51b26-108">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="51b26-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="51b26-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51b26-109">Properties</span></span>
|<span data-ttu-id="51b26-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51b26-110">Property</span></span>|<span data-ttu-id="51b26-111">種類</span><span class="sxs-lookup"><span data-stu-id="51b26-111">Type</span></span>|<span data-ttu-id="51b26-112">説明</span><span class="sxs-lookup"><span data-stu-id="51b26-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51b26-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="51b26-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="51b26-114">String</span><span class="sxs-lookup"><span data-stu-id="51b26-114">String</span></span>|<span data-ttu-id="51b26-115">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="51b26-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="51b26-116">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="51b26-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="51b26-117">address</span><span class="sxs-lookup"><span data-stu-id="51b26-117">address</span></span>|<span data-ttu-id="51b26-118">String</span><span class="sxs-lookup"><span data-stu-id="51b26-118">String</span></span>|<span data-ttu-id="51b26-119">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="51b26-119">Address.</span></span> <span data-ttu-id="51b26-120">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="51b26-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="51b26-121">port</span><span class="sxs-lookup"><span data-stu-id="51b26-121">port</span></span>|<span data-ttu-id="51b26-122">Int32</span><span class="sxs-lookup"><span data-stu-id="51b26-122">Int32</span></span>|<span data-ttu-id="51b26-123">ポートです。</span><span class="sxs-lookup"><span data-stu-id="51b26-123">Port.</span></span> <span data-ttu-id="51b26-124">有効な値は[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から 0 から 65535 までの継承</span><span class="sxs-lookup"><span data-stu-id="51b26-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="51b26-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="51b26-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="51b26-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="51b26-126">Boolean</span></span>|<span data-ttu-id="51b26-127">ローカル アドレスに対してプロキシ サーバーをバイパスします。</span><span class="sxs-lookup"><span data-stu-id="51b26-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51b26-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51b26-128">Relationships</span></span>
<span data-ttu-id="51b26-129">なし</span><span class="sxs-lookup"><span data-stu-id="51b26-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51b26-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51b26-130">JSON Representation</span></span>
<span data-ttu-id="51b26-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51b26-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```





