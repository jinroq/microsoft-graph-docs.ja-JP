---
title: vpnDnsRule リソースの種類
description: VPN の DNS ルール定義します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae6141cc0579840a23a28be2dce951c160f90248
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425583"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="07b98-103">vpnDnsRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="07b98-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="07b98-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07b98-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07b98-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07b98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07b98-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="07b98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07b98-107">VPN の DNS ルール定義します。</span><span class="sxs-lookup"><span data-stu-id="07b98-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="07b98-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07b98-108">Properties</span></span>
|<span data-ttu-id="07b98-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07b98-109">Property</span></span>|<span data-ttu-id="07b98-110">型</span><span class="sxs-lookup"><span data-stu-id="07b98-110">Type</span></span>|<span data-ttu-id="07b98-111">説明</span><span class="sxs-lookup"><span data-stu-id="07b98-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07b98-112">name</span><span class="sxs-lookup"><span data-stu-id="07b98-112">name</span></span>|<span data-ttu-id="07b98-113">String</span><span class="sxs-lookup"><span data-stu-id="07b98-113">String</span></span>|<span data-ttu-id="07b98-114">名前です。</span><span class="sxs-lookup"><span data-stu-id="07b98-114">Name.</span></span>|
|<span data-ttu-id="07b98-115">サーバー</span><span class="sxs-lookup"><span data-stu-id="07b98-115">servers</span></span>|<span data-ttu-id="07b98-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="07b98-116">String collection</span></span>|<span data-ttu-id="07b98-117">サーバーです。</span><span class="sxs-lookup"><span data-stu-id="07b98-117">Servers.</span></span>|
|<span data-ttu-id="07b98-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="07b98-118">proxyServerUri</span></span>|<span data-ttu-id="07b98-119">String</span><span class="sxs-lookup"><span data-stu-id="07b98-119">String</span></span>|<span data-ttu-id="07b98-120">プロキシ サーバーの Uri。</span><span class="sxs-lookup"><span data-stu-id="07b98-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="07b98-121">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="07b98-121">autoTrigger</span></span>|<span data-ttu-id="07b98-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="07b98-122">Boolean</span></span>|<span data-ttu-id="07b98-123">VPN への接続に自動的にデバイスがこのドメインに接続する場合: 既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="07b98-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="07b98-124">persistent</span><span class="sxs-lookup"><span data-stu-id="07b98-124">persistent</span></span>|<span data-ttu-id="07b98-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="07b98-125">Boolean</span></span>|<span data-ttu-id="07b98-126">VPN が接続されていない場合でもこの規則をアクティブにしておく既定値は False。</span><span class="sxs-lookup"><span data-stu-id="07b98-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="07b98-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07b98-127">Relationships</span></span>
<span data-ttu-id="07b98-128">なし</span><span class="sxs-lookup"><span data-stu-id="07b98-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07b98-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07b98-129">JSON Representation</span></span>
<span data-ttu-id="07b98-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="07b98-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```




