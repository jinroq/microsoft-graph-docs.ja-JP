---
title: ネットワーク接続リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 7dfc055c7603adc8d60908df58ce3995927316cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072649"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="b2f05-104">ネットワーク接続リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2f05-104">networkConnection resource type</span></span>

 > <span data-ttu-id="b2f05-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2f05-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2f05-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2f05-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2f05-107">アラートに関連するネットワーク接続に関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b2f05-107">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="b2f05-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2f05-108">Properties</span></span>

| <span data-ttu-id="b2f05-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2f05-109">Property</span></span>   | <span data-ttu-id="b2f05-110">型</span><span class="sxs-lookup"><span data-stu-id="b2f05-110">Type</span></span>|<span data-ttu-id="b2f05-111">説明</span><span class="sxs-lookup"><span data-stu-id="b2f05-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2f05-112">applicationName</span><span class="sxs-lookup"><span data-stu-id="b2f05-112">applicationName</span></span>|<span data-ttu-id="b2f05-113">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-113">String</span></span>|<span data-ttu-id="b2f05-114">ネットワーク接続 (たとえば、Facebook、SMTP など) を管理するアプリケーションの名前です。</span><span class="sxs-lookup"><span data-stu-id="b2f05-114">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="b2f05-115">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="b2f05-115">destinationAddress</span></span>|<span data-ttu-id="b2f05-116">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-116">String</span></span>|<span data-ttu-id="b2f05-117">宛先 IP アドレス (ネットワーク接続)。</span><span class="sxs-lookup"><span data-stu-id="b2f05-117">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="b2f05-118">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="b2f05-118">destinationDomain</span></span>|<span data-ttu-id="b2f05-119">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-119">String</span></span>|<span data-ttu-id="b2f05-120">リンク先の URL のリンク先のドメイン部分です。</span><span class="sxs-lookup"><span data-stu-id="b2f05-120">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="b2f05-121">(たとえば ' www.contoso.com')。</span><span class="sxs-lookup"><span data-stu-id="b2f05-121">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="b2f05-122">destinationPort</span><span class="sxs-lookup"><span data-stu-id="b2f05-122">destinationPort</span></span>|<span data-ttu-id="b2f05-123">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-123">String</span></span>|<span data-ttu-id="b2f05-124">宛先ポート (ネットワーク接続)。</span><span class="sxs-lookup"><span data-stu-id="b2f05-124">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="b2f05-125">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="b2f05-125">destinationUrl</span></span>|<span data-ttu-id="b2f05-126">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-126">String</span></span>|<span data-ttu-id="b2f05-127">ネットワークの接続の URL または URI 文字列のパラメーターを除外します。</span><span class="sxs-lookup"><span data-stu-id="b2f05-127">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="b2f05-128">(たとえば ' www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="b2f05-128">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="b2f05-129">方向</span><span class="sxs-lookup"><span data-stu-id="b2f05-129">direction</span></span>|<span data-ttu-id="b2f05-130">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="b2f05-130">connectionDirection</span></span>|<span data-ttu-id="b2f05-131">ネットワーク接続の方向です。</span><span class="sxs-lookup"><span data-stu-id="b2f05-131">Network connection direction.</span></span> <span data-ttu-id="b2f05-132">可能な値は、`unknown`、`inbound`、`outbound` です。</span><span class="sxs-lookup"><span data-stu-id="b2f05-132">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="b2f05-133">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="b2f05-133">domainRegisteredDateTime</span></span>|<span data-ttu-id="b2f05-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2f05-134">DateTimeOffset</span></span>|<span data-ttu-id="b2f05-135">移行先のドメインが登録された日付です。</span><span class="sxs-lookup"><span data-stu-id="b2f05-135">Date when the destination domain was registered.</span></span> <span data-ttu-id="b2f05-136">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="b2f05-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b2f05-137">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b2f05-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b2f05-138">localDnsName</span><span class="sxs-lookup"><span data-stu-id="b2f05-138">localDnsName</span></span>|<span data-ttu-id="b2f05-139">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-139">String</span></span>|<span data-ttu-id="b2f05-140">ローカル DNS 名前解決などの場合に 'ホスト' ファイルが改ざんされて)、ホストのローカル DNS キャッシュに表示されています。</span><span class="sxs-lookup"><span data-stu-id="b2f05-140">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="b2f05-141">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="b2f05-141">natDestinationAddress</span></span>|<span data-ttu-id="b2f05-142">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-142">String</span></span>|<span data-ttu-id="b2f05-143">ネットワーク アドレス変換の宛先 IP アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="b2f05-143">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="b2f05-144">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="b2f05-144">natDestinationPort</span></span>|<span data-ttu-id="b2f05-145">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-145">String</span></span>|<span data-ttu-id="b2f05-146">ネットワーク アドレス変換の送信先のポートを示します。</span><span class="sxs-lookup"><span data-stu-id="b2f05-146">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="b2f05-147">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="b2f05-147">natSourceAddress</span></span>|<span data-ttu-id="b2f05-148">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-148">String</span></span>|<span data-ttu-id="b2f05-149">ネットワーク アドレス変換の送信元 IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="b2f05-149">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="b2f05-150">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="b2f05-150">natSourcePort</span></span>|<span data-ttu-id="b2f05-151">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-151">String</span></span>|<span data-ttu-id="b2f05-152">ネットワーク アドレス変換のソース ポートです。</span><span class="sxs-lookup"><span data-stu-id="b2f05-152">Network Address Translation source port.</span></span>|
|<span data-ttu-id="b2f05-153">protocol</span><span class="sxs-lookup"><span data-stu-id="b2f05-153">protocol</span></span>|[<span data-ttu-id="b2f05-154">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="b2f05-154">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="b2f05-155">ネットワーク プロトコルです。</span><span class="sxs-lookup"><span data-stu-id="b2f05-155">Network protocol.</span></span> <span data-ttu-id="b2f05-156">使用可能な値: `unknown`、 `ip`、 `icmp`、 `igmp`、 `ggp`、 `ipv4`、 `tcp`、 `pup`、 `udp`、 `idp`、 `ipv6`、 `ipv6RoutingHeader`、 `ipv6FragmentHeader`、 `ipSecEncapsulatingSecurityPayload`、 `ipSecAuthenticationHeader`、 `icmpV6`、 `ipv6NoNextHeader`、 `ipv6DestinationOptions`、 `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="b2f05-156">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="b2f05-157">riskScore</span><span class="sxs-lookup"><span data-stu-id="b2f05-157">riskScore</span></span>|<span data-ttu-id="b2f05-158">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-158">String</span></span>|<span data-ttu-id="b2f05-159">プロバイダー生成された計算されるスコアのネットワーク接続の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b2f05-159">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="b2f05-160">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b2f05-160">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="b2f05-161">発信元アドレス</span><span class="sxs-lookup"><span data-stu-id="b2f05-161">sourceAddress</span></span>|<span data-ttu-id="b2f05-162">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-162">String</span></span>|<span data-ttu-id="b2f05-163">(ネットワーク接続) の IP アドレスをソース (つまり原点)。</span><span class="sxs-lookup"><span data-stu-id="b2f05-163">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="b2f05-164">sourcePort</span><span class="sxs-lookup"><span data-stu-id="b2f05-164">sourcePort</span></span>|<span data-ttu-id="b2f05-165">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-165">String</span></span>|<span data-ttu-id="b2f05-166">(ネットワーク接続) の IP ポートをソース (つまり原点)。</span><span class="sxs-lookup"><span data-stu-id="b2f05-166">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="b2f05-167">status</span><span class="sxs-lookup"><span data-stu-id="b2f05-167">status</span></span>|<span data-ttu-id="b2f05-168">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="b2f05-168">connectionStatus</span></span>|<span data-ttu-id="b2f05-169">ネットワーク接続の状態です。</span><span class="sxs-lookup"><span data-stu-id="b2f05-169">Network connection status.</span></span> <span data-ttu-id="b2f05-170">可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="b2f05-170">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="b2f05-171">urlParameters</span><span class="sxs-lookup"><span data-stu-id="b2f05-171">urlParameters</span></span>|<span data-ttu-id="b2f05-172">String</span><span class="sxs-lookup"><span data-stu-id="b2f05-172">String</span></span>|<span data-ttu-id="b2f05-173">リンク先の URL のパラメーター (サフィックス) にします。</span><span class="sxs-lookup"><span data-stu-id="b2f05-173">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2f05-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2f05-174">JSON representation</span></span>

<span data-ttu-id="b2f05-175">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b2f05-175">The following is a JSON representation of the resource.</span></span>

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
