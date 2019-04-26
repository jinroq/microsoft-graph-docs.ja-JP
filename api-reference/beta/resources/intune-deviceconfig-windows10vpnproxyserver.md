---
title: windows10VpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 212bafa99a51e269716978cafa4fcf274dd76579
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572025"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="4b031-103">windows10VpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b031-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="4b031-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b031-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b031-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b031-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b031-106">VPN プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="4b031-106">VPN Proxy Server.</span></span>


<span data-ttu-id="4b031-107">[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4b031-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b031-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b031-108">Properties</span></span>
|<span data-ttu-id="4b031-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b031-109">Property</span></span>|<span data-ttu-id="4b031-110">型</span><span class="sxs-lookup"><span data-stu-id="4b031-110">Type</span></span>|<span data-ttu-id="4b031-111">説明</span><span class="sxs-lookup"><span data-stu-id="4b031-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b031-112">自動構成 scripturl</span><span class="sxs-lookup"><span data-stu-id="4b031-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="4b031-113">String</span><span class="sxs-lookup"><span data-stu-id="4b031-113">String</span></span>|<span data-ttu-id="4b031-114">プロキシの自動構成スクリプトの url。</span><span class="sxs-lookup"><span data-stu-id="4b031-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="4b031-115">[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4b031-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4b031-116">address</span><span class="sxs-lookup"><span data-stu-id="4b031-116">address</span></span>|<span data-ttu-id="4b031-117">String</span><span class="sxs-lookup"><span data-stu-id="4b031-117">String</span></span>|<span data-ttu-id="4b031-118">連絡先.</span><span class="sxs-lookup"><span data-stu-id="4b031-118">Address.</span></span> <span data-ttu-id="4b031-119">[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4b031-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4b031-120">ポート</span><span class="sxs-lookup"><span data-stu-id="4b031-120">port</span></span>|<span data-ttu-id="4b031-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4b031-121">Int32</span></span>|<span data-ttu-id="4b031-122">ポート.</span><span class="sxs-lookup"><span data-stu-id="4b031-122">Port.</span></span> <span data-ttu-id="4b031-123">[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)から継承された有効な値 0 ~ 65535</span><span class="sxs-lookup"><span data-stu-id="4b031-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4b031-124">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="4b031-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="4b031-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b031-125">Boolean</span></span>|<span data-ttu-id="4b031-126">ローカルアドレスにはプロキシサーバーを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="4b031-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b031-127">関係</span><span class="sxs-lookup"><span data-stu-id="4b031-127">Relationships</span></span>
<span data-ttu-id="4b031-128">なし</span><span class="sxs-lookup"><span data-stu-id="4b031-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b031-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b031-129">JSON Representation</span></span>
<span data-ttu-id="4b031-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b031-130">Here is a JSON representation of the resource.</span></span>
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





