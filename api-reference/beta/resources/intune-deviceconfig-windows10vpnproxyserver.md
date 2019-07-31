---
title: windows10VpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 95c0d475f3000c31592fb8b1363a4b39258b98ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969143"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="e8303-103">windows10VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8303-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="e8303-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8303-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8303-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8303-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8303-106">VPN プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="e8303-106">VPN Proxy Server.</span></span>


<span data-ttu-id="e8303-107">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e8303-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8303-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8303-108">Properties</span></span>
|<span data-ttu-id="e8303-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8303-109">Property</span></span>|<span data-ttu-id="e8303-110">型</span><span class="sxs-lookup"><span data-stu-id="e8303-110">Type</span></span>|<span data-ttu-id="e8303-111">説明</span><span class="sxs-lookup"><span data-stu-id="e8303-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8303-112">自動構成 Scripturl</span><span class="sxs-lookup"><span data-stu-id="e8303-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="e8303-113">String</span><span class="sxs-lookup"><span data-stu-id="e8303-113">String</span></span>|<span data-ttu-id="e8303-114">プロキシの自動構成スクリプトの url。</span><span class="sxs-lookup"><span data-stu-id="e8303-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="e8303-115">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e8303-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="e8303-116">address</span><span class="sxs-lookup"><span data-stu-id="e8303-116">address</span></span>|<span data-ttu-id="e8303-117">String</span><span class="sxs-lookup"><span data-stu-id="e8303-117">String</span></span>|<span data-ttu-id="e8303-118">連絡先.</span><span class="sxs-lookup"><span data-stu-id="e8303-118">Address.</span></span> <span data-ttu-id="e8303-119">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e8303-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="e8303-120">ポート</span><span class="sxs-lookup"><span data-stu-id="e8303-120">port</span></span>|<span data-ttu-id="e8303-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e8303-121">Int32</span></span>|<span data-ttu-id="e8303-122">ポート.</span><span class="sxs-lookup"><span data-stu-id="e8303-122">Port.</span></span> <span data-ttu-id="e8303-123">[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承された有効な値 0 ~ 65535</span><span class="sxs-lookup"><span data-stu-id="e8303-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="e8303-124">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="e8303-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="e8303-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8303-125">Boolean</span></span>|<span data-ttu-id="e8303-126">ローカルアドレスにはプロキシサーバーを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="e8303-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8303-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8303-127">Relationships</span></span>
<span data-ttu-id="e8303-128">なし</span><span class="sxs-lookup"><span data-stu-id="e8303-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8303-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8303-129">JSON Representation</span></span>
<span data-ttu-id="e8303-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8303-130">Here is a JSON representation of the resource.</span></span>
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





