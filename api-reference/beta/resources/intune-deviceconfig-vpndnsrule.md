---
title: vpnDnsRule リソースの種類
description: VPN DNS ルールの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 983b30b1f724c3c8f76e967179c6fcdb1ff1fecb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367730"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="b52be-103">vpnDnsRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b52be-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="b52be-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b52be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b52be-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b52be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b52be-106">VPN DNS ルールの定義。</span><span class="sxs-lookup"><span data-stu-id="b52be-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b52be-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b52be-107">Properties</span></span>
|<span data-ttu-id="b52be-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b52be-108">Property</span></span>|<span data-ttu-id="b52be-109">型</span><span class="sxs-lookup"><span data-stu-id="b52be-109">Type</span></span>|<span data-ttu-id="b52be-110">説明</span><span class="sxs-lookup"><span data-stu-id="b52be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b52be-111">name</span><span class="sxs-lookup"><span data-stu-id="b52be-111">name</span></span>|<span data-ttu-id="b52be-112">String</span><span class="sxs-lookup"><span data-stu-id="b52be-112">String</span></span>|<span data-ttu-id="b52be-113">拡張子.</span><span class="sxs-lookup"><span data-stu-id="b52be-113">Name.</span></span>|
|<span data-ttu-id="b52be-114">サーバ</span><span class="sxs-lookup"><span data-stu-id="b52be-114">servers</span></span>|<span data-ttu-id="b52be-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b52be-115">String collection</span></span>|<span data-ttu-id="b52be-116">サーバ.</span><span class="sxs-lookup"><span data-stu-id="b52be-116">Servers.</span></span>|
|<span data-ttu-id="b52be-117">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="b52be-117">proxyServerUri</span></span>|<span data-ttu-id="b52be-118">String</span><span class="sxs-lookup"><span data-stu-id="b52be-118">String</span></span>|<span data-ttu-id="b52be-119">プロキシサーバーの Uri。</span><span class="sxs-lookup"><span data-stu-id="b52be-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="b52be-120">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="b52be-120">autoTrigger</span></span>|<span data-ttu-id="b52be-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="b52be-121">Boolean</span></span>|<span data-ttu-id="b52be-122">デバイスがこのドメインに接続されている場合は、自動的に VPN に接続します。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="b52be-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="b52be-123">引き続き</span><span class="sxs-lookup"><span data-stu-id="b52be-123">persistent</span></span>|<span data-ttu-id="b52be-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b52be-124">Boolean</span></span>|<span data-ttu-id="b52be-125">VPN が接続されていない場合も、このルールをアクティブにします。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="b52be-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="b52be-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b52be-126">Relationships</span></span>
<span data-ttu-id="b52be-127">なし</span><span class="sxs-lookup"><span data-stu-id="b52be-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b52be-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b52be-128">JSON Representation</span></span>
<span data-ttu-id="b52be-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b52be-129">Here is a JSON representation of the resource.</span></span>
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



