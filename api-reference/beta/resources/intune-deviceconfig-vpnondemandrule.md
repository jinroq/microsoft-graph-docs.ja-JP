---
title: vpnOnDemandRule リソースの種類
description: VPN のオンデマンドルールの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7b562f9f1be09c5214905e67b2a8ac604e03f20
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367667"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="7a0f5-103">vpnOnDemandRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a0f5-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="7a0f5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a0f5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a0f5-106">VPN のオンデマンドルールの定義。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="7a0f5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a0f5-107">Properties</span></span>
|<span data-ttu-id="7a0f5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a0f5-108">Property</span></span>|<span data-ttu-id="7a0f5-109">型</span><span class="sxs-lookup"><span data-stu-id="7a0f5-109">Type</span></span>|<span data-ttu-id="7a0f5-110">説明</span><span class="sxs-lookup"><span data-stu-id="7a0f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a0f5-111">ssid</span><span class="sxs-lookup"><span data-stu-id="7a0f5-111">ssids</span></span>|<span data-ttu-id="7a0f5-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7a0f5-112">String collection</span></span>|<span data-ttu-id="7a0f5-113">ネットワークサービスセット識別子 (Ssid)。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="7a0f5-114">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="7a0f5-114">dnsSearchDomains</span></span>|<span data-ttu-id="7a0f5-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7a0f5-115">String collection</span></span>|<span data-ttu-id="7a0f5-116">DNS 検索ドメイン。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="7a0f5-117">probeUrl</span><span class="sxs-lookup"><span data-stu-id="7a0f5-117">probeUrl</span></span>|<span data-ttu-id="7a0f5-118">String</span><span class="sxs-lookup"><span data-stu-id="7a0f5-118">String</span></span>|<span data-ttu-id="7a0f5-119">プローブする URL。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-119">A URL to probe.</span></span> <span data-ttu-id="7a0f5-120">リダイレクトされていない (200 HTTP 状態コードを返す) この URL が正常に取得された場合、このルールは一致します。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="7a0f5-121">action</span><span class="sxs-lookup"><span data-stu-id="7a0f5-121">action</span></span>|[<span data-ttu-id="7a0f5-122">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="7a0f5-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="7a0f5-123">Action.</span><span class="sxs-lookup"><span data-stu-id="7a0f5-123">Action.</span></span> <span data-ttu-id="7a0f5-124">使用可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="7a0f5-125">domainAction</span><span class="sxs-lookup"><span data-stu-id="7a0f5-125">domainAction</span></span>|[<span data-ttu-id="7a0f5-126">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="7a0f5-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="7a0f5-127">ドメインアクション (アクションが接続を評価する場合にのみ該当)。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="7a0f5-128">可能な値は、`connectIfNeeded`、`neverConnect` です。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="7a0f5-129">ドメイン</span><span class="sxs-lookup"><span data-stu-id="7a0f5-129">domains</span></span>|<span data-ttu-id="7a0f5-130">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7a0f5-130">String collection</span></span>|<span data-ttu-id="7a0f5-131">ドメイン (アクションが接続を評価する場合にのみ該当)。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="7a0f5-132">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="7a0f5-132">probeRequiredUrl</span></span>|<span data-ttu-id="7a0f5-133">String</span><span class="sxs-lookup"><span data-stu-id="7a0f5-133">String</span></span>|<span data-ttu-id="7a0f5-134">必要な Url をプローブします (アクションが接続を評価する場合にのみ適用され、必要に応じて、DomainAction が connect である)。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a0f5-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a0f5-135">Relationships</span></span>
<span data-ttu-id="7a0f5-136">なし</span><span class="sxs-lookup"><span data-stu-id="7a0f5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a0f5-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a0f5-137">JSON Representation</span></span>
<span data-ttu-id="7a0f5-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a0f5-138">Here is a JSON representation of the resource.</span></span>
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



