---
title: vpnOnDemandRule リソースの種類
description: VPN のオンデマンドルールの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb17bb1ec1af12f89ea1ab5470cf6a2d808868c4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944587"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="bcff9-103">vpnOnDemandRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bcff9-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="bcff9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcff9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcff9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcff9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcff9-106">VPN のオンデマンドルールの定義。</span><span class="sxs-lookup"><span data-stu-id="bcff9-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="bcff9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcff9-107">Properties</span></span>
|<span data-ttu-id="bcff9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcff9-108">Property</span></span>|<span data-ttu-id="bcff9-109">型</span><span class="sxs-lookup"><span data-stu-id="bcff9-109">Type</span></span>|<span data-ttu-id="bcff9-110">説明</span><span class="sxs-lookup"><span data-stu-id="bcff9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcff9-111">ssid</span><span class="sxs-lookup"><span data-stu-id="bcff9-111">ssids</span></span>|<span data-ttu-id="bcff9-112">String collection</span><span class="sxs-lookup"><span data-stu-id="bcff9-112">String collection</span></span>|<span data-ttu-id="bcff9-113">ネットワークサービスセット識別子 (Ssid)。</span><span class="sxs-lookup"><span data-stu-id="bcff9-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="bcff9-114">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="bcff9-114">dnsSearchDomains</span></span>|<span data-ttu-id="bcff9-115">String collection</span><span class="sxs-lookup"><span data-stu-id="bcff9-115">String collection</span></span>|<span data-ttu-id="bcff9-116">DNS 検索ドメイン。</span><span class="sxs-lookup"><span data-stu-id="bcff9-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="bcff9-117">probeUrl</span><span class="sxs-lookup"><span data-stu-id="bcff9-117">probeUrl</span></span>|<span data-ttu-id="bcff9-118">String</span><span class="sxs-lookup"><span data-stu-id="bcff9-118">String</span></span>|<span data-ttu-id="bcff9-119">プローブする URL。</span><span class="sxs-lookup"><span data-stu-id="bcff9-119">A URL to probe.</span></span> <span data-ttu-id="bcff9-120">リダイレクトされていない (200 HTTP 状態コードを返す) この URL が正常に取得された場合、このルールは一致します。</span><span class="sxs-lookup"><span data-stu-id="bcff9-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="bcff9-121">action</span><span class="sxs-lookup"><span data-stu-id="bcff9-121">action</span></span>|[<span data-ttu-id="bcff9-122">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="bcff9-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="bcff9-123">Action.</span><span class="sxs-lookup"><span data-stu-id="bcff9-123">Action.</span></span> <span data-ttu-id="bcff9-124">使用可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。</span><span class="sxs-lookup"><span data-stu-id="bcff9-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="bcff9-125">domainAction</span><span class="sxs-lookup"><span data-stu-id="bcff9-125">domainAction</span></span>|[<span data-ttu-id="bcff9-126">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="bcff9-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="bcff9-127">ドメインアクション (アクションが接続を評価する場合にのみ該当)。</span><span class="sxs-lookup"><span data-stu-id="bcff9-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="bcff9-128">可能な値は、`connectIfNeeded`、`neverConnect` です。</span><span class="sxs-lookup"><span data-stu-id="bcff9-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="bcff9-129">ドメイン</span><span class="sxs-lookup"><span data-stu-id="bcff9-129">domains</span></span>|<span data-ttu-id="bcff9-130">String collection</span><span class="sxs-lookup"><span data-stu-id="bcff9-130">String collection</span></span>|<span data-ttu-id="bcff9-131">ドメイン (アクションが接続を評価する場合にのみ該当)。</span><span class="sxs-lookup"><span data-stu-id="bcff9-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="bcff9-132">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="bcff9-132">probeRequiredUrl</span></span>|<span data-ttu-id="bcff9-133">String</span><span class="sxs-lookup"><span data-stu-id="bcff9-133">String</span></span>|<span data-ttu-id="bcff9-134">必要な Url をプローブします (アクションが接続を評価する場合にのみ適用され、必要に応じて、DomainAction が connect である)。</span><span class="sxs-lookup"><span data-stu-id="bcff9-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcff9-135">関係</span><span class="sxs-lookup"><span data-stu-id="bcff9-135">Relationships</span></span>
<span data-ttu-id="bcff9-136">なし</span><span class="sxs-lookup"><span data-stu-id="bcff9-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bcff9-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bcff9-137">JSON Representation</span></span>
<span data-ttu-id="bcff9-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bcff9-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```




