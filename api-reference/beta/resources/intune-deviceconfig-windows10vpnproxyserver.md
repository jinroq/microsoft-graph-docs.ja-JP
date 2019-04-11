---
title: windows10VpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 212bafa99a51e269716978cafa4fcf274dd76579
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797901"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="3fdc2-103">windows10VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3fdc2-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="3fdc2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fdc2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fdc2-106">VPN プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-106">VPN Proxy Server.</span></span>


<span data-ttu-id="3fdc2-107">[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3fdc2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3fdc2-108">Properties</span></span>
|<span data-ttu-id="3fdc2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3fdc2-109">Property</span></span>|<span data-ttu-id="3fdc2-110">型</span><span class="sxs-lookup"><span data-stu-id="3fdc2-110">Type</span></span>|<span data-ttu-id="3fdc2-111">説明</span><span class="sxs-lookup"><span data-stu-id="3fdc2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fdc2-112">自動構成 scripturl</span><span class="sxs-lookup"><span data-stu-id="3fdc2-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="3fdc2-113">文字列</span><span class="sxs-lookup"><span data-stu-id="3fdc2-113">String</span></span>|<span data-ttu-id="3fdc2-114">プロキシの自動構成スクリプトの url。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="3fdc2-115">[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3fdc2-116">address</span><span class="sxs-lookup"><span data-stu-id="3fdc2-116">address</span></span>|<span data-ttu-id="3fdc2-117">String</span><span class="sxs-lookup"><span data-stu-id="3fdc2-117">String</span></span>|<span data-ttu-id="3fdc2-118">連絡先.</span><span class="sxs-lookup"><span data-stu-id="3fdc2-118">Address.</span></span> <span data-ttu-id="3fdc2-119">[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3fdc2-120">ポート</span><span class="sxs-lookup"><span data-stu-id="3fdc2-120">port</span></span>|<span data-ttu-id="3fdc2-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3fdc2-121">Int32</span></span>|<span data-ttu-id="3fdc2-122">ポート.</span><span class="sxs-lookup"><span data-stu-id="3fdc2-122">Port.</span></span> <span data-ttu-id="3fdc2-123">[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承された有効な値 0 ~ 65535</span><span class="sxs-lookup"><span data-stu-id="3fdc2-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3fdc2-124">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="3fdc2-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="3fdc2-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fdc2-125">Boolean</span></span>|<span data-ttu-id="3fdc2-126">ローカルアドレスにはプロキシサーバーを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fdc2-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3fdc2-127">Relationships</span></span>
<span data-ttu-id="3fdc2-128">なし</span><span class="sxs-lookup"><span data-stu-id="3fdc2-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fdc2-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3fdc2-129">JSON Representation</span></span>
<span data-ttu-id="3fdc2-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3fdc2-130">Here is a JSON representation of the resource.</span></span>
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





