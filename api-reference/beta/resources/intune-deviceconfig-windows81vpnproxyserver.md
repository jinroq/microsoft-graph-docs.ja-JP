---
title: windows81VpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
ms.openlocfilehash: 27100dd3faecc9ba20a4bcc28985c56c9cb409c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067315"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="fe9aa-103">windows81VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe9aa-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="fe9aa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe9aa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe9aa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe9aa-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-107">VPN Proxy Server.</span></span>

<span data-ttu-id="fe9aa-108">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fe9aa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe9aa-109">Properties</span></span>
|<span data-ttu-id="fe9aa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe9aa-110">Property</span></span>|<span data-ttu-id="fe9aa-111">型</span><span class="sxs-lookup"><span data-stu-id="fe9aa-111">Type</span></span>|<span data-ttu-id="fe9aa-112">説明</span><span class="sxs-lookup"><span data-stu-id="fe9aa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe9aa-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="fe9aa-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="fe9aa-114">String</span><span class="sxs-lookup"><span data-stu-id="fe9aa-114">String</span></span>|<span data-ttu-id="fe9aa-115">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="fe9aa-116">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="fe9aa-117">address</span><span class="sxs-lookup"><span data-stu-id="fe9aa-117">address</span></span>|<span data-ttu-id="fe9aa-118">String</span><span class="sxs-lookup"><span data-stu-id="fe9aa-118">String</span></span>|<span data-ttu-id="fe9aa-119">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-119">Address.</span></span> <span data-ttu-id="fe9aa-120">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="fe9aa-121">port</span><span class="sxs-lookup"><span data-stu-id="fe9aa-121">port</span></span>|<span data-ttu-id="fe9aa-122">Int32</span><span class="sxs-lookup"><span data-stu-id="fe9aa-122">Int32</span></span>|<span data-ttu-id="fe9aa-123">ポートです。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-123">Port.</span></span> <span data-ttu-id="fe9aa-124">有効な値は[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から 0 から 65535 までの継承</span><span class="sxs-lookup"><span data-stu-id="fe9aa-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="fe9aa-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="fe9aa-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="fe9aa-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="fe9aa-126">Boolean</span></span>|<span data-ttu-id="fe9aa-127">プロキシの設定を自動的に検出します。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="fe9aa-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="fe9aa-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="fe9aa-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="fe9aa-129">Boolean</span></span>|<span data-ttu-id="fe9aa-130">ローカル アドレスに対してプロキシ サーバーをバイパスします。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe9aa-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fe9aa-131">Relationships</span></span>
<span data-ttu-id="fe9aa-132">なし</span><span class="sxs-lookup"><span data-stu-id="fe9aa-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fe9aa-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe9aa-133">JSON Representation</span></span>
<span data-ttu-id="fe9aa-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fe9aa-134">Here is a JSON representation of the resource.</span></span>
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





