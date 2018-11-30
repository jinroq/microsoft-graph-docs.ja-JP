---
title: ネットワーク接続リソースの種類
description: アラートに関連するネットワーク接続に関するステートフルな情報が含まれています。
ms.openlocfilehash: e3352cbda430412691285c209c566fb379045681
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023898"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="fc139-103">ネットワーク接続リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc139-103">networkConnection resource type</span></span>

<span data-ttu-id="fc139-104">アラートに関連するネットワーク接続に関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc139-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="fc139-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc139-105">Properties</span></span>

| <span data-ttu-id="fc139-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc139-106">Property</span></span>   | <span data-ttu-id="fc139-107">型</span><span class="sxs-lookup"><span data-stu-id="fc139-107">Type</span></span>|<span data-ttu-id="fc139-108">説明</span><span class="sxs-lookup"><span data-stu-id="fc139-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc139-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="fc139-109">applicationName</span></span>|<span data-ttu-id="fc139-110">String</span><span class="sxs-lookup"><span data-stu-id="fc139-110">String</span></span>|<span data-ttu-id="fc139-111">ネットワーク接続 (たとえば、Facebook、SMTP など) を管理するアプリケーションの名前です。</span><span class="sxs-lookup"><span data-stu-id="fc139-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="fc139-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="fc139-112">destinationAddress</span></span>|<span data-ttu-id="fc139-113">String</span><span class="sxs-lookup"><span data-stu-id="fc139-113">String</span></span>|<span data-ttu-id="fc139-114">宛先 IP アドレス (ネットワーク接続)。</span><span class="sxs-lookup"><span data-stu-id="fc139-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="fc139-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="fc139-115">destinationDomain</span></span>|<span data-ttu-id="fc139-116">String</span><span class="sxs-lookup"><span data-stu-id="fc139-116">String</span></span>|<span data-ttu-id="fc139-117">リンク先の URL のリンク先のドメイン部分です。</span><span class="sxs-lookup"><span data-stu-id="fc139-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="fc139-118">(たとえば ' www.contoso.com')。</span><span class="sxs-lookup"><span data-stu-id="fc139-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="fc139-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="fc139-119">destinationPort</span></span>|<span data-ttu-id="fc139-120">String</span><span class="sxs-lookup"><span data-stu-id="fc139-120">String</span></span>|<span data-ttu-id="fc139-121">宛先ポート (ネットワーク接続)。</span><span class="sxs-lookup"><span data-stu-id="fc139-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="fc139-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="fc139-122">destinationUrl</span></span>|<span data-ttu-id="fc139-123">String</span><span class="sxs-lookup"><span data-stu-id="fc139-123">String</span></span>|<span data-ttu-id="fc139-124">ネットワークの接続の URL または URI 文字列のパラメーターを除外します。</span><span class="sxs-lookup"><span data-stu-id="fc139-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="fc139-125">(たとえば ' www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="fc139-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="fc139-126">方向</span><span class="sxs-lookup"><span data-stu-id="fc139-126">direction</span></span>|<span data-ttu-id="fc139-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="fc139-127">connectionDirection</span></span>|<span data-ttu-id="fc139-128">ネットワーク接続の方向です。</span><span class="sxs-lookup"><span data-stu-id="fc139-128">Network connection direction.</span></span> <span data-ttu-id="fc139-129">可能な値は、`unknown`、`inbound`、`outbound` です。</span><span class="sxs-lookup"><span data-stu-id="fc139-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="fc139-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="fc139-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="fc139-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc139-131">DateTimeOffset</span></span>|<span data-ttu-id="fc139-132">移行先のドメインが登録された日付です。</span><span class="sxs-lookup"><span data-stu-id="fc139-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="fc139-133">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="fc139-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fc139-134">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fc139-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fc139-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="fc139-135">localDnsName</span></span>|<span data-ttu-id="fc139-136">String</span><span class="sxs-lookup"><span data-stu-id="fc139-136">String</span></span>|<span data-ttu-id="fc139-137">ローカル DNS 名前解決などの場合に 'ホスト' ファイルが改ざんされて)、ホストのローカル DNS キャッシュに表示されています。</span><span class="sxs-lookup"><span data-stu-id="fc139-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="fc139-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="fc139-138">natDestinationAddress</span></span>|<span data-ttu-id="fc139-139">String</span><span class="sxs-lookup"><span data-stu-id="fc139-139">String</span></span>|<span data-ttu-id="fc139-140">ネットワーク アドレス変換の宛先 IP アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="fc139-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="fc139-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="fc139-141">natDestinationPort</span></span>|<span data-ttu-id="fc139-142">String</span><span class="sxs-lookup"><span data-stu-id="fc139-142">String</span></span>|<span data-ttu-id="fc139-143">ネットワーク アドレス変換の送信先のポートを示します。</span><span class="sxs-lookup"><span data-stu-id="fc139-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="fc139-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="fc139-144">natSourceAddress</span></span>|<span data-ttu-id="fc139-145">String</span><span class="sxs-lookup"><span data-stu-id="fc139-145">String</span></span>|<span data-ttu-id="fc139-146">ネットワーク アドレス変換の送信元 IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="fc139-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="fc139-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="fc139-147">natSourcePort</span></span>|<span data-ttu-id="fc139-148">String</span><span class="sxs-lookup"><span data-stu-id="fc139-148">String</span></span>|<span data-ttu-id="fc139-149">ネットワーク アドレス変換のソース ポートです。</span><span class="sxs-lookup"><span data-stu-id="fc139-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="fc139-150">protocol</span><span class="sxs-lookup"><span data-stu-id="fc139-150">protocol</span></span>|[<span data-ttu-id="fc139-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="fc139-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="fc139-152">ネットワーク プロトコルです。</span><span class="sxs-lookup"><span data-stu-id="fc139-152">Network protocol.</span></span> <span data-ttu-id="fc139-153">使用可能な値: `unknown`、 `ip`、 `icmp`、 `igmp`、 `ggp`、 `ipv4`、 `tcp`、 `pup`、 `udp`、 `idp`、 `ipv6`、 `ipv6RoutingHeader`、 `ipv6FragmentHeader`、 `ipSecEncapsulatingSecurityPayload`、 `ipSecAuthenticationHeader`、 `icmpV6`、 `ipv6NoNextHeader`、 `ipv6DestinationOptions`、 `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="fc139-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="fc139-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="fc139-154">riskScore</span></span>|<span data-ttu-id="fc139-155">String</span><span class="sxs-lookup"><span data-stu-id="fc139-155">String</span></span>|<span data-ttu-id="fc139-156">プロバイダー生成された計算されるスコアのネットワーク接続の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fc139-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="fc139-157">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="fc139-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="fc139-158">発信元アドレス</span><span class="sxs-lookup"><span data-stu-id="fc139-158">sourceAddress</span></span>|<span data-ttu-id="fc139-159">String</span><span class="sxs-lookup"><span data-stu-id="fc139-159">String</span></span>|<span data-ttu-id="fc139-160">(ネットワーク接続) の IP アドレスをソース (つまり原点)。</span><span class="sxs-lookup"><span data-stu-id="fc139-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="fc139-161">sourcePort</span><span class="sxs-lookup"><span data-stu-id="fc139-161">sourcePort</span></span>|<span data-ttu-id="fc139-162">String</span><span class="sxs-lookup"><span data-stu-id="fc139-162">String</span></span>|<span data-ttu-id="fc139-163">(ネットワーク接続) の IP ポートをソース (つまり原点)。</span><span class="sxs-lookup"><span data-stu-id="fc139-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="fc139-164">status</span><span class="sxs-lookup"><span data-stu-id="fc139-164">status</span></span>|<span data-ttu-id="fc139-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="fc139-165">connectionStatus</span></span>|<span data-ttu-id="fc139-166">ネットワーク接続の状態です。</span><span class="sxs-lookup"><span data-stu-id="fc139-166">Network connection status.</span></span> <span data-ttu-id="fc139-167">可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="fc139-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="fc139-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="fc139-168">urlParameters</span></span>|<span data-ttu-id="fc139-169">String</span><span class="sxs-lookup"><span data-stu-id="fc139-169">String</span></span>|<span data-ttu-id="fc139-170">リンク先の URL のパラメーター (サフィックス) にします。</span><span class="sxs-lookup"><span data-stu-id="fc139-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc139-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc139-171">JSON representation</span></span>

<span data-ttu-id="fc139-172">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fc139-172">The following is a JSON representation of the resource.</span></span>

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