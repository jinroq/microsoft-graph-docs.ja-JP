---
title: vpnProxyServer リソースの種類
description: VPN プロキシ サーバーです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 676e56771f021a79179e268280f5e3190754eef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425674"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="c18c2-103">vpnProxyServer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c18c2-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="c18c2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c18c2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c18c2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c18c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c18c2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c18c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c18c2-107">VPN プロキシ サーバーです。</span><span class="sxs-lookup"><span data-stu-id="c18c2-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="c18c2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c18c2-108">Properties</span></span>
|<span data-ttu-id="c18c2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c18c2-109">Property</span></span>|<span data-ttu-id="c18c2-110">型</span><span class="sxs-lookup"><span data-stu-id="c18c2-110">Type</span></span>|<span data-ttu-id="c18c2-111">説明</span><span class="sxs-lookup"><span data-stu-id="c18c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c18c2-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="c18c2-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="c18c2-113">String</span><span class="sxs-lookup"><span data-stu-id="c18c2-113">String</span></span>|<span data-ttu-id="c18c2-114">プロキシの自動構成スクリプトの url です。</span><span class="sxs-lookup"><span data-stu-id="c18c2-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="c18c2-115">address</span><span class="sxs-lookup"><span data-stu-id="c18c2-115">address</span></span>|<span data-ttu-id="c18c2-116">String</span><span class="sxs-lookup"><span data-stu-id="c18c2-116">String</span></span>|<span data-ttu-id="c18c2-117">アドレスです。</span><span class="sxs-lookup"><span data-stu-id="c18c2-117">Address.</span></span>|
|<span data-ttu-id="c18c2-118">port</span><span class="sxs-lookup"><span data-stu-id="c18c2-118">port</span></span>|<span data-ttu-id="c18c2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="c18c2-119">Int32</span></span>|<span data-ttu-id="c18c2-120">ポートです。</span><span class="sxs-lookup"><span data-stu-id="c18c2-120">Port.</span></span> <span data-ttu-id="c18c2-121">0 から 65535 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="c18c2-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="c18c2-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c18c2-122">Relationships</span></span>
<span data-ttu-id="c18c2-123">なし</span><span class="sxs-lookup"><span data-stu-id="c18c2-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c18c2-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c18c2-124">JSON Representation</span></span>
<span data-ttu-id="c18c2-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c18c2-125">Here is a JSON representation of the resource.</span></span>
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




