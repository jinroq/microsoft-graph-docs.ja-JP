---
title: vpnOnDemandRule リソースの種類
description: VPN のオンデマンドルールの定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1bccd015e45291b344e7c77df4ac5c0a0af07d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161587"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="2501a-103">vpnOnDemandRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2501a-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="2501a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2501a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2501a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2501a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2501a-106">VPN のオンデマンドルールの定義。</span><span class="sxs-lookup"><span data-stu-id="2501a-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2501a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2501a-107">Properties</span></span>
|<span data-ttu-id="2501a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2501a-108">Property</span></span>|<span data-ttu-id="2501a-109">型</span><span class="sxs-lookup"><span data-stu-id="2501a-109">Type</span></span>|<span data-ttu-id="2501a-110">説明</span><span class="sxs-lookup"><span data-stu-id="2501a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2501a-111">ssid</span><span class="sxs-lookup"><span data-stu-id="2501a-111">ssids</span></span>|<span data-ttu-id="2501a-112">String collection</span><span class="sxs-lookup"><span data-stu-id="2501a-112">String collection</span></span>|<span data-ttu-id="2501a-113">ネットワークサービスセット識別子 (ssid)。</span><span class="sxs-lookup"><span data-stu-id="2501a-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="2501a-114">dnssearchdomains</span><span class="sxs-lookup"><span data-stu-id="2501a-114">dnsSearchDomains</span></span>|<span data-ttu-id="2501a-115">String collection</span><span class="sxs-lookup"><span data-stu-id="2501a-115">String collection</span></span>|<span data-ttu-id="2501a-116">DNS 検索ドメイン。</span><span class="sxs-lookup"><span data-stu-id="2501a-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="2501a-117">probeUrl</span><span class="sxs-lookup"><span data-stu-id="2501a-117">probeUrl</span></span>|<span data-ttu-id="2501a-118">String</span><span class="sxs-lookup"><span data-stu-id="2501a-118">String</span></span>|<span data-ttu-id="2501a-119">プローブする URL。</span><span class="sxs-lookup"><span data-stu-id="2501a-119">A URL to probe.</span></span> <span data-ttu-id="2501a-120">リダイレクトされていない (200 HTTP 状態コードを返す) この URL が正常に取得された場合、このルールは一致します。</span><span class="sxs-lookup"><span data-stu-id="2501a-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="2501a-121">action</span><span class="sxs-lookup"><span data-stu-id="2501a-121">action</span></span>|[<span data-ttu-id="2501a-122">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="2501a-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="2501a-123">Action.</span><span class="sxs-lookup"><span data-stu-id="2501a-123">Action.</span></span> <span data-ttu-id="2501a-124">使用可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。</span><span class="sxs-lookup"><span data-stu-id="2501a-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="2501a-125">domainaction</span><span class="sxs-lookup"><span data-stu-id="2501a-125">domainAction</span></span>|[<span data-ttu-id="2501a-126">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="2501a-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="2501a-127">ドメインアクション (アクションが接続を評価する場合にのみ該当)。</span><span class="sxs-lookup"><span data-stu-id="2501a-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="2501a-128">使用可能な値は、`connectIfNeeded`、`neverConnect` です。</span><span class="sxs-lookup"><span data-stu-id="2501a-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="2501a-129">ドメイン</span><span class="sxs-lookup"><span data-stu-id="2501a-129">domains</span></span>|<span data-ttu-id="2501a-130">String collection</span><span class="sxs-lookup"><span data-stu-id="2501a-130">String collection</span></span>|<span data-ttu-id="2501a-131">ドメイン (アクションが接続を評価する場合にのみ該当)。</span><span class="sxs-lookup"><span data-stu-id="2501a-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="2501a-132">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="2501a-132">probeRequiredUrl</span></span>|<span data-ttu-id="2501a-133">String</span><span class="sxs-lookup"><span data-stu-id="2501a-133">String</span></span>|<span data-ttu-id="2501a-134">必要な Url をプローブします (アクションが接続を評価する場合にのみ適用され、必要に応じて、domainaction が connect である)。</span><span class="sxs-lookup"><span data-stu-id="2501a-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2501a-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2501a-135">Relationships</span></span>
<span data-ttu-id="2501a-136">なし</span><span class="sxs-lookup"><span data-stu-id="2501a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2501a-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2501a-137">JSON Representation</span></span>
<span data-ttu-id="2501a-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2501a-138">Here is a JSON representation of the resource.</span></span>
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




