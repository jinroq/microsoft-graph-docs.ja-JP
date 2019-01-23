---
title: windows10VpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f8975a08e60105c37e0959ac72e24a1dd639cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407124"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="ccaf5-103">windows10VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ccaf5-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="ccaf5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ccaf5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccaf5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccaf5-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-107">VPN Proxy Server.</span></span>


<span data-ttu-id="ccaf5-108">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ccaf5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccaf5-109">Properties</span></span>
|<span data-ttu-id="ccaf5-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccaf5-110">Property</span></span>|<span data-ttu-id="ccaf5-111">型</span><span class="sxs-lookup"><span data-stu-id="ccaf5-111">Type</span></span>|<span data-ttu-id="ccaf5-112">説明</span><span class="sxs-lookup"><span data-stu-id="ccaf5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccaf5-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="ccaf5-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="ccaf5-114">String</span><span class="sxs-lookup"><span data-stu-id="ccaf5-114">String</span></span>|<span data-ttu-id="ccaf5-115">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="ccaf5-116">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="ccaf5-117">address</span><span class="sxs-lookup"><span data-stu-id="ccaf5-117">address</span></span>|<span data-ttu-id="ccaf5-118">String</span><span class="sxs-lookup"><span data-stu-id="ccaf5-118">String</span></span>|<span data-ttu-id="ccaf5-119">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-119">Address.</span></span> <span data-ttu-id="ccaf5-120">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="ccaf5-121">port</span><span class="sxs-lookup"><span data-stu-id="ccaf5-121">port</span></span>|<span data-ttu-id="ccaf5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ccaf5-122">Int32</span></span>|<span data-ttu-id="ccaf5-123">ポートです。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-123">Port.</span></span> <span data-ttu-id="ccaf5-124">有効な値は[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から 0 から 65535 までの継承</span><span class="sxs-lookup"><span data-stu-id="ccaf5-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="ccaf5-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="ccaf5-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="ccaf5-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccaf5-126">Boolean</span></span>|<span data-ttu-id="ccaf5-127">ローカル アドレスに対してプロキシ サーバーをバイパスします。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccaf5-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ccaf5-128">Relationships</span></span>
<span data-ttu-id="ccaf5-129">なし</span><span class="sxs-lookup"><span data-stu-id="ccaf5-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccaf5-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ccaf5-130">JSON Representation</span></span>
<span data-ttu-id="ccaf5-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ccaf5-131">Here is a JSON representation of the resource.</span></span>
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




