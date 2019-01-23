---
title: windows81VpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a400ed128a80e6fae11f090f7cdd445fe8c174b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398892"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="d9a5a-103">windows81VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9a5a-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="d9a5a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9a5a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9a5a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9a5a-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-107">VPN Proxy Server.</span></span>


<span data-ttu-id="d9a5a-108">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9a5a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9a5a-109">Properties</span></span>
|<span data-ttu-id="d9a5a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9a5a-110">Property</span></span>|<span data-ttu-id="d9a5a-111">型</span><span class="sxs-lookup"><span data-stu-id="d9a5a-111">Type</span></span>|<span data-ttu-id="d9a5a-112">説明</span><span class="sxs-lookup"><span data-stu-id="d9a5a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a5a-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="d9a5a-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="d9a5a-114">String</span><span class="sxs-lookup"><span data-stu-id="d9a5a-114">String</span></span>|<span data-ttu-id="d9a5a-115">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="d9a5a-116">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="d9a5a-117">address</span><span class="sxs-lookup"><span data-stu-id="d9a5a-117">address</span></span>|<span data-ttu-id="d9a5a-118">String</span><span class="sxs-lookup"><span data-stu-id="d9a5a-118">String</span></span>|<span data-ttu-id="d9a5a-119">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-119">Address.</span></span> <span data-ttu-id="d9a5a-120">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="d9a5a-121">port</span><span class="sxs-lookup"><span data-stu-id="d9a5a-121">port</span></span>|<span data-ttu-id="d9a5a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="d9a5a-122">Int32</span></span>|<span data-ttu-id="d9a5a-123">ポートです。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-123">Port.</span></span> <span data-ttu-id="d9a5a-124">有効な値は[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から 0 から 65535 までの継承</span><span class="sxs-lookup"><span data-stu-id="d9a5a-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="d9a5a-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="d9a5a-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="d9a5a-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a5a-126">Boolean</span></span>|<span data-ttu-id="d9a5a-127">プロキシの設定を自動的に検出します。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="d9a5a-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="d9a5a-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="d9a5a-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a5a-129">Boolean</span></span>|<span data-ttu-id="d9a5a-130">ローカル アドレスに対してプロキシ サーバーをバイパスします。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9a5a-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d9a5a-131">Relationships</span></span>
<span data-ttu-id="d9a5a-132">なし</span><span class="sxs-lookup"><span data-stu-id="d9a5a-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9a5a-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9a5a-133">JSON Representation</span></span>
<span data-ttu-id="d9a5a-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d9a5a-134">Here is a JSON representation of the resource.</span></span>
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




