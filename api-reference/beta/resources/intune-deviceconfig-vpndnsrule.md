---
title: vpndnsrule リソースの種類
description: VPN DNS ルールの定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 545c0dd8a84f19888452261e350a9b347061595c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158507"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="27a4b-103">vpndnsrule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27a4b-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="27a4b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27a4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27a4b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27a4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27a4b-106">VPN DNS ルールの定義。</span><span class="sxs-lookup"><span data-stu-id="27a4b-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="27a4b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27a4b-107">Properties</span></span>
|<span data-ttu-id="27a4b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27a4b-108">Property</span></span>|<span data-ttu-id="27a4b-109">型</span><span class="sxs-lookup"><span data-stu-id="27a4b-109">Type</span></span>|<span data-ttu-id="27a4b-110">説明</span><span class="sxs-lookup"><span data-stu-id="27a4b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27a4b-111">name</span><span class="sxs-lookup"><span data-stu-id="27a4b-111">name</span></span>|<span data-ttu-id="27a4b-112">String</span><span class="sxs-lookup"><span data-stu-id="27a4b-112">String</span></span>|<span data-ttu-id="27a4b-113">拡張子.</span><span class="sxs-lookup"><span data-stu-id="27a4b-113">Name.</span></span>|
|<span data-ttu-id="27a4b-114">サーバー</span><span class="sxs-lookup"><span data-stu-id="27a4b-114">servers</span></span>|<span data-ttu-id="27a4b-115">String collection</span><span class="sxs-lookup"><span data-stu-id="27a4b-115">String collection</span></span>|<span data-ttu-id="27a4b-116">サーバ.</span><span class="sxs-lookup"><span data-stu-id="27a4b-116">Servers.</span></span>|
|<span data-ttu-id="27a4b-117">proxyserveruri</span><span class="sxs-lookup"><span data-stu-id="27a4b-117">proxyServerUri</span></span>|<span data-ttu-id="27a4b-118">String</span><span class="sxs-lookup"><span data-stu-id="27a4b-118">String</span></span>|<span data-ttu-id="27a4b-119">プロキシサーバーの Uri。</span><span class="sxs-lookup"><span data-stu-id="27a4b-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="27a4b-120">autotrigger</span><span class="sxs-lookup"><span data-stu-id="27a4b-120">autoTrigger</span></span>|<span data-ttu-id="27a4b-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="27a4b-121">Boolean</span></span>|<span data-ttu-id="27a4b-122">デバイスがこのドメインに接続されている場合は、自動的に VPN に接続します。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="27a4b-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="27a4b-123">persistent</span><span class="sxs-lookup"><span data-stu-id="27a4b-123">persistent</span></span>|<span data-ttu-id="27a4b-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="27a4b-124">Boolean</span></span>|<span data-ttu-id="27a4b-125">VPN が接続されていない場合も、このルールをアクティブにします。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="27a4b-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="27a4b-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27a4b-126">Relationships</span></span>
<span data-ttu-id="27a4b-127">なし</span><span class="sxs-lookup"><span data-stu-id="27a4b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27a4b-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27a4b-128">JSON Representation</span></span>
<span data-ttu-id="27a4b-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="27a4b-129">Here is a JSON representation of the resource.</span></span>
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




