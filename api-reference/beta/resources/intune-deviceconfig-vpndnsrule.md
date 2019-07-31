---
title: vpnDnsRule リソースの種類
description: VPN DNS ルールの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76182d87ec04220ed126165676961e11722f17ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969514"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="89850-103">vpnDnsRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89850-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="89850-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89850-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89850-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="89850-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89850-106">VPN DNS ルールの定義。</span><span class="sxs-lookup"><span data-stu-id="89850-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="89850-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89850-107">Properties</span></span>
|<span data-ttu-id="89850-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89850-108">Property</span></span>|<span data-ttu-id="89850-109">型</span><span class="sxs-lookup"><span data-stu-id="89850-109">Type</span></span>|<span data-ttu-id="89850-110">説明</span><span class="sxs-lookup"><span data-stu-id="89850-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89850-111">name</span><span class="sxs-lookup"><span data-stu-id="89850-111">name</span></span>|<span data-ttu-id="89850-112">String</span><span class="sxs-lookup"><span data-stu-id="89850-112">String</span></span>|<span data-ttu-id="89850-113">拡張子.</span><span class="sxs-lookup"><span data-stu-id="89850-113">Name.</span></span>|
|<span data-ttu-id="89850-114">サーバ</span><span class="sxs-lookup"><span data-stu-id="89850-114">servers</span></span>|<span data-ttu-id="89850-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="89850-115">String collection</span></span>|<span data-ttu-id="89850-116">サーバ.</span><span class="sxs-lookup"><span data-stu-id="89850-116">Servers.</span></span>|
|<span data-ttu-id="89850-117">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="89850-117">proxyServerUri</span></span>|<span data-ttu-id="89850-118">String</span><span class="sxs-lookup"><span data-stu-id="89850-118">String</span></span>|<span data-ttu-id="89850-119">プロキシサーバーの Uri。</span><span class="sxs-lookup"><span data-stu-id="89850-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="89850-120">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="89850-120">autoTrigger</span></span>|<span data-ttu-id="89850-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="89850-121">Boolean</span></span>|<span data-ttu-id="89850-122">デバイスがこのドメインに接続されている場合は、自動的に VPN に接続します。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="89850-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="89850-123">引き続き</span><span class="sxs-lookup"><span data-stu-id="89850-123">persistent</span></span>|<span data-ttu-id="89850-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="89850-124">Boolean</span></span>|<span data-ttu-id="89850-125">VPN が接続されていない場合も、このルールをアクティブにします。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="89850-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="89850-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="89850-126">Relationships</span></span>
<span data-ttu-id="89850-127">なし</span><span class="sxs-lookup"><span data-stu-id="89850-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89850-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89850-128">JSON Representation</span></span>
<span data-ttu-id="89850-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="89850-129">Here is a JSON representation of the resource.</span></span>
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





