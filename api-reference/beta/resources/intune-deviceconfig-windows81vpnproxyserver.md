---
title: windows81VpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26f15e8e2b6982c322ffc78cb9d6270b08bcbc3c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944244"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="1e13a-103">windows81VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e13a-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="1e13a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e13a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e13a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e13a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e13a-106">VPN プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="1e13a-106">VPN Proxy Server.</span></span>


<span data-ttu-id="1e13a-107">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1e13a-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e13a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e13a-108">Properties</span></span>
|<span data-ttu-id="1e13a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e13a-109">Property</span></span>|<span data-ttu-id="1e13a-110">型</span><span class="sxs-lookup"><span data-stu-id="1e13a-110">Type</span></span>|<span data-ttu-id="1e13a-111">説明</span><span class="sxs-lookup"><span data-stu-id="1e13a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e13a-112">自動構成 Scripturl</span><span class="sxs-lookup"><span data-stu-id="1e13a-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="1e13a-113">String</span><span class="sxs-lookup"><span data-stu-id="1e13a-113">String</span></span>|<span data-ttu-id="1e13a-114">プロキシの自動構成スクリプトの url。</span><span class="sxs-lookup"><span data-stu-id="1e13a-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="1e13a-115">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1e13a-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="1e13a-116">address</span><span class="sxs-lookup"><span data-stu-id="1e13a-116">address</span></span>|<span data-ttu-id="1e13a-117">String</span><span class="sxs-lookup"><span data-stu-id="1e13a-117">String</span></span>|<span data-ttu-id="1e13a-118">連絡先.</span><span class="sxs-lookup"><span data-stu-id="1e13a-118">Address.</span></span> <span data-ttu-id="1e13a-119">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1e13a-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="1e13a-120">ポート</span><span class="sxs-lookup"><span data-stu-id="1e13a-120">port</span></span>|<span data-ttu-id="1e13a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="1e13a-121">Int32</span></span>|<span data-ttu-id="1e13a-122">ポート.</span><span class="sxs-lookup"><span data-stu-id="1e13a-122">Port.</span></span> <span data-ttu-id="1e13a-123">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承された有効な値 0 ~ 65535</span><span class="sxs-lookup"><span data-stu-id="1e13a-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="1e13a-124">自動的に検出する Proxysettings</span><span class="sxs-lookup"><span data-stu-id="1e13a-124">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="1e13a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e13a-125">Boolean</span></span>|<span data-ttu-id="1e13a-126">プロキシの設定を自動的に検出します。</span><span class="sxs-lookup"><span data-stu-id="1e13a-126">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="1e13a-127">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="1e13a-127">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="1e13a-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e13a-128">Boolean</span></span>|<span data-ttu-id="1e13a-129">ローカルアドレスにはプロキシサーバーを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="1e13a-129">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e13a-130">関係</span><span class="sxs-lookup"><span data-stu-id="1e13a-130">Relationships</span></span>
<span data-ttu-id="1e13a-131">なし</span><span class="sxs-lookup"><span data-stu-id="1e13a-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e13a-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e13a-132">JSON Representation</span></span>
<span data-ttu-id="1e13a-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e13a-133">Here is a JSON representation of the resource.</span></span>
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




