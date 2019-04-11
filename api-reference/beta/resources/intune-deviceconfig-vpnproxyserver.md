---
title: vpnProxyServer リソースの種類
description: VPN プロキシサーバー。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c711f02dc0b4f7e44ff1bd54669ed9befb73e42a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807645"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="97303-103">vpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97303-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="97303-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97303-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97303-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97303-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97303-106">VPN プロキシサーバー。</span><span class="sxs-lookup"><span data-stu-id="97303-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="97303-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97303-107">Properties</span></span>
|<span data-ttu-id="97303-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97303-108">Property</span></span>|<span data-ttu-id="97303-109">型</span><span class="sxs-lookup"><span data-stu-id="97303-109">Type</span></span>|<span data-ttu-id="97303-110">説明</span><span class="sxs-lookup"><span data-stu-id="97303-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97303-111">自動構成 scripturl</span><span class="sxs-lookup"><span data-stu-id="97303-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="97303-112">文字列</span><span class="sxs-lookup"><span data-stu-id="97303-112">String</span></span>|<span data-ttu-id="97303-113">プロキシの自動構成スクリプトの url。</span><span class="sxs-lookup"><span data-stu-id="97303-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="97303-114">address</span><span class="sxs-lookup"><span data-stu-id="97303-114">address</span></span>|<span data-ttu-id="97303-115">String</span><span class="sxs-lookup"><span data-stu-id="97303-115">String</span></span>|<span data-ttu-id="97303-116">連絡先.</span><span class="sxs-lookup"><span data-stu-id="97303-116">Address.</span></span>|
|<span data-ttu-id="97303-117">ポート</span><span class="sxs-lookup"><span data-stu-id="97303-117">port</span></span>|<span data-ttu-id="97303-118">Int32</span><span class="sxs-lookup"><span data-stu-id="97303-118">Int32</span></span>|<span data-ttu-id="97303-119">ポート.</span><span class="sxs-lookup"><span data-stu-id="97303-119">Port.</span></span> <span data-ttu-id="97303-120">有効な値は 0 ~ 65535</span><span class="sxs-lookup"><span data-stu-id="97303-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="97303-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97303-121">Relationships</span></span>
<span data-ttu-id="97303-122">なし</span><span class="sxs-lookup"><span data-stu-id="97303-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97303-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97303-123">JSON Representation</span></span>
<span data-ttu-id="97303-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97303-124">Here is a JSON representation of the resource.</span></span>
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





