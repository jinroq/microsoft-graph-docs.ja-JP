---
title: windows81VpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b694206fd65bad46c9176a9fc01586f00237bdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834714"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="70462-103">windows81VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70462-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="70462-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="70462-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70462-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70462-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70462-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="70462-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70462-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="70462-107">VPN Proxy Server.</span></span>

<span data-ttu-id="70462-108">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="70462-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="70462-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70462-109">Properties</span></span>
|<span data-ttu-id="70462-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70462-110">Property</span></span>|<span data-ttu-id="70462-111">種類</span><span class="sxs-lookup"><span data-stu-id="70462-111">Type</span></span>|<span data-ttu-id="70462-112">説明</span><span class="sxs-lookup"><span data-stu-id="70462-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70462-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="70462-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="70462-114">String</span><span class="sxs-lookup"><span data-stu-id="70462-114">String</span></span>|<span data-ttu-id="70462-115">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="70462-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="70462-116">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="70462-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="70462-117">address</span><span class="sxs-lookup"><span data-stu-id="70462-117">address</span></span>|<span data-ttu-id="70462-118">String</span><span class="sxs-lookup"><span data-stu-id="70462-118">String</span></span>|<span data-ttu-id="70462-119">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="70462-119">Address.</span></span> <span data-ttu-id="70462-120">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="70462-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="70462-121">port</span><span class="sxs-lookup"><span data-stu-id="70462-121">port</span></span>|<span data-ttu-id="70462-122">Int32</span><span class="sxs-lookup"><span data-stu-id="70462-122">Int32</span></span>|<span data-ttu-id="70462-123">ポートです。</span><span class="sxs-lookup"><span data-stu-id="70462-123">Port.</span></span> <span data-ttu-id="70462-124">有効な値は[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から 0 から 65535 までの継承</span><span class="sxs-lookup"><span data-stu-id="70462-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="70462-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="70462-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="70462-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="70462-126">Boolean</span></span>|<span data-ttu-id="70462-127">プロキシの設定を自動的に検出します。</span><span class="sxs-lookup"><span data-stu-id="70462-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="70462-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="70462-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="70462-129">ブール型</span><span class="sxs-lookup"><span data-stu-id="70462-129">Boolean</span></span>|<span data-ttu-id="70462-130">ローカル アドレスに対してプロキシ サーバーをバイパスします。</span><span class="sxs-lookup"><span data-stu-id="70462-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70462-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="70462-131">Relationships</span></span>
<span data-ttu-id="70462-132">なし</span><span class="sxs-lookup"><span data-stu-id="70462-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="70462-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70462-133">JSON Representation</span></span>
<span data-ttu-id="70462-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="70462-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```





