---
title: vpnOnDemandRule リソースの種類
description: VPN オンデマンド ルール定義します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bd6e494975c8626a25380b3f037d702fb81e082b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875636"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="513b7-103">vpnOnDemandRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="513b7-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="513b7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="513b7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="513b7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="513b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="513b7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="513b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="513b7-107">VPN オンデマンド ルール定義します。</span><span class="sxs-lookup"><span data-stu-id="513b7-107">VPN On-Demand Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="513b7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="513b7-108">Properties</span></span>
|<span data-ttu-id="513b7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="513b7-109">Property</span></span>|<span data-ttu-id="513b7-110">種類</span><span class="sxs-lookup"><span data-stu-id="513b7-110">Type</span></span>|<span data-ttu-id="513b7-111">説明</span><span class="sxs-lookup"><span data-stu-id="513b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="513b7-112">ssid</span><span class="sxs-lookup"><span data-stu-id="513b7-112">ssids</span></span>|<span data-ttu-id="513b7-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="513b7-113">String collection</span></span>|<span data-ttu-id="513b7-114">ネットワーク サービスでは、識別子 (Ssid) を設定します。</span><span class="sxs-lookup"><span data-stu-id="513b7-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="513b7-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="513b7-115">dnsSearchDomains</span></span>|<span data-ttu-id="513b7-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="513b7-116">String collection</span></span>|<span data-ttu-id="513b7-117">DNS ドメインを検索します。</span><span class="sxs-lookup"><span data-stu-id="513b7-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="513b7-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="513b7-118">probeUrl</span></span>|<span data-ttu-id="513b7-119">String</span><span class="sxs-lookup"><span data-stu-id="513b7-119">String</span></span>|<span data-ttu-id="513b7-120">プローブへの URL です。</span><span class="sxs-lookup"><span data-stu-id="513b7-120">A URL to probe.</span></span> <span data-ttu-id="513b7-121">この URL は、正常に場合、リダイレクトには、(HTTP ステータス コード 200 を返す) をフェッチ、この規則に一致します。</span><span class="sxs-lookup"><span data-stu-id="513b7-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="513b7-122">action</span><span class="sxs-lookup"><span data-stu-id="513b7-122">action</span></span>|[<span data-ttu-id="513b7-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="513b7-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="513b7-124">アクションです。</span><span class="sxs-lookup"><span data-stu-id="513b7-124">Action.</span></span> <span data-ttu-id="513b7-125">可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。</span><span class="sxs-lookup"><span data-stu-id="513b7-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="513b7-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="513b7-126">domainAction</span></span>|[<span data-ttu-id="513b7-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="513b7-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="513b7-128">ドメインのアクション (アクションは、接続を評価するときにのみ該当する)。</span><span class="sxs-lookup"><span data-stu-id="513b7-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="513b7-129">使用可能な値は、`connectIfNeeded`、`neverConnect` です。</span><span class="sxs-lookup"><span data-stu-id="513b7-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="513b7-130">ドメイン</span><span class="sxs-lookup"><span data-stu-id="513b7-130">domains</span></span>|<span data-ttu-id="513b7-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="513b7-131">String collection</span></span>|<span data-ttu-id="513b7-132">(操作は、接続を評価するときにのみ該当する) のドメインです。</span><span class="sxs-lookup"><span data-stu-id="513b7-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="513b7-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="513b7-133">probeRequiredUrl</span></span>|<span data-ttu-id="513b7-134">String</span><span class="sxs-lookup"><span data-stu-id="513b7-134">String</span></span>|<span data-ttu-id="513b7-135">(操作は、接続を評価し、必要な場合に DomainAction を接続するときにのみ該当する) が必要な Url をプローブします。</span><span class="sxs-lookup"><span data-stu-id="513b7-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="513b7-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="513b7-136">Relationships</span></span>
<span data-ttu-id="513b7-137">なし</span><span class="sxs-lookup"><span data-stu-id="513b7-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="513b7-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="513b7-138">JSON Representation</span></span>
<span data-ttu-id="513b7-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="513b7-139">Here is a JSON representation of the resource.</span></span>
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





