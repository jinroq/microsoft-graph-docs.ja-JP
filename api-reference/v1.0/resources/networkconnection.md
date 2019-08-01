---
title: networkConnection リソースの種類
description: 通知に関連するネットワーク接続に関するステートフルな情報を含みます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 25750b5484558c53ab03d3001bc2b8bafa307524
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035995"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="d8f59-103">networkConnection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8f59-103">networkConnection resource type</span></span>

<span data-ttu-id="d8f59-104">通知に関連するネットワーク接続に関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="d8f59-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="d8f59-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8f59-105">Properties</span></span>

| <span data-ttu-id="d8f59-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8f59-106">Property</span></span>   | <span data-ttu-id="d8f59-107">型</span><span class="sxs-lookup"><span data-stu-id="d8f59-107">Type</span></span>|<span data-ttu-id="d8f59-108">説明</span><span class="sxs-lookup"><span data-stu-id="d8f59-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8f59-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="d8f59-109">applicationName</span></span>|<span data-ttu-id="d8f59-110">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-110">String</span></span>|<span data-ttu-id="d8f59-111">ネットワーク接続を管理しているアプリケーションの名前 (例: Facebook、SMTP など)。</span><span class="sxs-lookup"><span data-stu-id="d8f59-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="d8f59-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="d8f59-112">destinationAddress</span></span>|<span data-ttu-id="d8f59-113">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-113">String</span></span>|<span data-ttu-id="d8f59-114">宛先 IP アドレス (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="d8f59-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="d8f59-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="d8f59-115">destinationDomain</span></span>|<span data-ttu-id="d8f59-116">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-116">String</span></span>|<span data-ttu-id="d8f59-117">宛先 URL の宛先ドメイン部分。</span><span class="sxs-lookup"><span data-stu-id="d8f59-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="d8f59-118">(' www.contoso.com ' など)。</span><span class="sxs-lookup"><span data-stu-id="d8f59-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="d8f59-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="d8f59-119">destinationPort</span></span>|<span data-ttu-id="d8f59-120">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-120">String</span></span>|<span data-ttu-id="d8f59-121">宛先ポート (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="d8f59-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="d8f59-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="d8f59-122">destinationUrl</span></span>|<span data-ttu-id="d8f59-123">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-123">String</span></span>|<span data-ttu-id="d8f59-124">ネットワーク接続 URL/URI 文字列。パラメーターを除外します。</span><span class="sxs-lookup"><span data-stu-id="d8f59-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="d8f59-125">(' www.contoso.com/products/default.html ' など)</span><span class="sxs-lookup"><span data-stu-id="d8f59-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="d8f59-126">direction</span><span class="sxs-lookup"><span data-stu-id="d8f59-126">direction</span></span>|<span data-ttu-id="d8f59-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="d8f59-127">connectionDirection</span></span>|<span data-ttu-id="d8f59-128">ネットワーク接続の方向。</span><span class="sxs-lookup"><span data-stu-id="d8f59-128">Network connection direction.</span></span> <span data-ttu-id="d8f59-129">可能な値は、`unknown`、`inbound`、`outbound` です。</span><span class="sxs-lookup"><span data-stu-id="d8f59-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="d8f59-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="d8f59-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="d8f59-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8f59-131">DateTimeOffset</span></span>|<span data-ttu-id="d8f59-132">宛先ドメインが登録された日付。</span><span class="sxs-lookup"><span data-stu-id="d8f59-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="d8f59-133">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d8f59-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8f59-134">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d8f59-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d8f59-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="d8f59-135">localDnsName</span></span>|<span data-ttu-id="d8f59-136">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-136">String</span></span>|<span data-ttu-id="d8f59-137">ホストのローカル DNS キャッシュに表示されるローカル DNS 名解決方法 (たとえば、' hosts ' ファイルが改ざんされた場合)。</span><span class="sxs-lookup"><span data-stu-id="d8f59-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="d8f59-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="d8f59-138">natDestinationAddress</span></span>|<span data-ttu-id="d8f59-139">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-139">String</span></span>|<span data-ttu-id="d8f59-140">ネットワークアドレス変換先 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="d8f59-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="d8f59-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="d8f59-141">natDestinationPort</span></span>|<span data-ttu-id="d8f59-142">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-142">String</span></span>|<span data-ttu-id="d8f59-143">ネットワークアドレス変換先ポート。</span><span class="sxs-lookup"><span data-stu-id="d8f59-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="d8f59-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="d8f59-144">natSourceAddress</span></span>|<span data-ttu-id="d8f59-145">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-145">String</span></span>|<span data-ttu-id="d8f59-146">ネットワークアドレス変換の送信元 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="d8f59-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="d8f59-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="d8f59-147">natSourcePort</span></span>|<span data-ttu-id="d8f59-148">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-148">String</span></span>|<span data-ttu-id="d8f59-149">ネットワークアドレス変換元ポート。</span><span class="sxs-lookup"><span data-stu-id="d8f59-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="d8f59-150">プロトコール</span><span class="sxs-lookup"><span data-stu-id="d8f59-150">protocol</span></span>|[<span data-ttu-id="d8f59-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="d8f59-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="d8f59-152">ネットワークプロトコル。</span><span class="sxs-lookup"><span data-stu-id="d8f59-152">Network protocol.</span></span> <span data-ttu-id="d8f59-153">可能な値: `unknown`、 `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader`、、、、、、、、、、、、 `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="d8f59-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="d8f59-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="d8f59-154">riskScore</span></span>|<span data-ttu-id="d8f59-155">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-155">String</span></span>|<span data-ttu-id="d8f59-156">プロバイダーが生成/計算したネットワーク接続のリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="d8f59-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="d8f59-157">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="d8f59-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="d8f59-158">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="d8f59-158">sourceAddress</span></span>|<span data-ttu-id="d8f59-159">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-159">String</span></span>|<span data-ttu-id="d8f59-160">ソース (起点) IP アドレス (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="d8f59-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="d8f59-161">sourcePort</span><span class="sxs-lookup"><span data-stu-id="d8f59-161">sourcePort</span></span>|<span data-ttu-id="d8f59-162">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-162">String</span></span>|<span data-ttu-id="d8f59-163">ソース (起点) IP ポート (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="d8f59-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="d8f59-164">status</span><span class="sxs-lookup"><span data-stu-id="d8f59-164">status</span></span>|<span data-ttu-id="d8f59-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="d8f59-165">connectionStatus</span></span>|<span data-ttu-id="d8f59-166">ネットワーク接続の状態。</span><span class="sxs-lookup"><span data-stu-id="d8f59-166">Network connection status.</span></span> <span data-ttu-id="d8f59-167">可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="d8f59-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="d8f59-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="d8f59-168">urlParameters</span></span>|<span data-ttu-id="d8f59-169">String</span><span class="sxs-lookup"><span data-stu-id="d8f59-169">String</span></span>|<span data-ttu-id="d8f59-170">宛先 URL のパラメーター (サフィックス)。</span><span class="sxs-lookup"><span data-stu-id="d8f59-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8f59-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8f59-171">JSON representation</span></span>

<span data-ttu-id="d8f59-172">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d8f59-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
