---
title: vpnOnDemandRule リソースの種類
description: VPN オンデマンド ルール定義します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8164d1c12aeb172120bb9803d7f3dd98366ec948
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421460"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="c09e3-103">vpnOnDemandRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c09e3-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="c09e3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c09e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c09e3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c09e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c09e3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c09e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c09e3-107">VPN オンデマンド ルール定義します。</span><span class="sxs-lookup"><span data-stu-id="c09e3-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c09e3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c09e3-108">Properties</span></span>
|<span data-ttu-id="c09e3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c09e3-109">Property</span></span>|<span data-ttu-id="c09e3-110">型</span><span class="sxs-lookup"><span data-stu-id="c09e3-110">Type</span></span>|<span data-ttu-id="c09e3-111">説明</span><span class="sxs-lookup"><span data-stu-id="c09e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c09e3-112">ssid</span><span class="sxs-lookup"><span data-stu-id="c09e3-112">ssids</span></span>|<span data-ttu-id="c09e3-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c09e3-113">String collection</span></span>|<span data-ttu-id="c09e3-114">ネットワーク サービスでは、識別子 (Ssid) を設定します。</span><span class="sxs-lookup"><span data-stu-id="c09e3-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="c09e3-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="c09e3-115">dnsSearchDomains</span></span>|<span data-ttu-id="c09e3-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c09e3-116">String collection</span></span>|<span data-ttu-id="c09e3-117">DNS ドメインを検索します。</span><span class="sxs-lookup"><span data-stu-id="c09e3-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="c09e3-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="c09e3-118">probeUrl</span></span>|<span data-ttu-id="c09e3-119">String</span><span class="sxs-lookup"><span data-stu-id="c09e3-119">String</span></span>|<span data-ttu-id="c09e3-120">プローブへの URL です。</span><span class="sxs-lookup"><span data-stu-id="c09e3-120">A URL to probe.</span></span> <span data-ttu-id="c09e3-121">この URL は、正常に場合、リダイレクトには、(HTTP ステータス コード 200 を返す) をフェッチ、この規則に一致します。</span><span class="sxs-lookup"><span data-stu-id="c09e3-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="c09e3-122">action</span><span class="sxs-lookup"><span data-stu-id="c09e3-122">action</span></span>|[<span data-ttu-id="c09e3-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="c09e3-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="c09e3-124">アクションです。</span><span class="sxs-lookup"><span data-stu-id="c09e3-124">Action.</span></span> <span data-ttu-id="c09e3-125">可能な値は、`connect`、`evaluateConnection`、`ignore`、`disconnect` です。</span><span class="sxs-lookup"><span data-stu-id="c09e3-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="c09e3-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="c09e3-126">domainAction</span></span>|[<span data-ttu-id="c09e3-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="c09e3-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="c09e3-128">ドメインのアクション (アクションは、接続を評価するときにのみ該当する)。</span><span class="sxs-lookup"><span data-stu-id="c09e3-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="c09e3-129">使用可能な値は、`connectIfNeeded`、`neverConnect` です。</span><span class="sxs-lookup"><span data-stu-id="c09e3-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="c09e3-130">ドメイン</span><span class="sxs-lookup"><span data-stu-id="c09e3-130">domains</span></span>|<span data-ttu-id="c09e3-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c09e3-131">String collection</span></span>|<span data-ttu-id="c09e3-132">(操作は、接続を評価するときにのみ該当する) のドメインです。</span><span class="sxs-lookup"><span data-stu-id="c09e3-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="c09e3-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="c09e3-133">probeRequiredUrl</span></span>|<span data-ttu-id="c09e3-134">String</span><span class="sxs-lookup"><span data-stu-id="c09e3-134">String</span></span>|<span data-ttu-id="c09e3-135">(操作は、接続を評価し、必要な場合に DomainAction を接続するときにのみ該当する) が必要な Url をプローブします。</span><span class="sxs-lookup"><span data-stu-id="c09e3-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c09e3-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c09e3-136">Relationships</span></span>
<span data-ttu-id="c09e3-137">なし</span><span class="sxs-lookup"><span data-stu-id="c09e3-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c09e3-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c09e3-138">JSON Representation</span></span>
<span data-ttu-id="c09e3-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c09e3-139">Here is a JSON representation of the resource.</span></span>
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




