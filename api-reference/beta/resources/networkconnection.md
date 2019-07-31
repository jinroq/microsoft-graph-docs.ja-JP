---
title: networkConnection リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 90e505abfb9256276d24b81c3d038b2b0882069a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966672"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="863b0-104">networkConnection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="863b0-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="863b0-105">通知に関連するネットワーク接続に関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="863b0-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="863b0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="863b0-106">Properties</span></span>

| <span data-ttu-id="863b0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="863b0-107">Property</span></span>   | <span data-ttu-id="863b0-108">型</span><span class="sxs-lookup"><span data-stu-id="863b0-108">Type</span></span>|<span data-ttu-id="863b0-109">説明</span><span class="sxs-lookup"><span data-stu-id="863b0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="863b0-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="863b0-110">applicationName</span></span>|<span data-ttu-id="863b0-111">String</span><span class="sxs-lookup"><span data-stu-id="863b0-111">String</span></span>|<span data-ttu-id="863b0-112">ネットワーク接続を管理しているアプリケーションの名前 (例: Facebook、SMTP など)。</span><span class="sxs-lookup"><span data-stu-id="863b0-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="863b0-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="863b0-113">destinationAddress</span></span>|<span data-ttu-id="863b0-114">String</span><span class="sxs-lookup"><span data-stu-id="863b0-114">String</span></span>|<span data-ttu-id="863b0-115">宛先 IP アドレス (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="863b0-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="863b0-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="863b0-116">destinationDomain</span></span>|<span data-ttu-id="863b0-117">String</span><span class="sxs-lookup"><span data-stu-id="863b0-117">String</span></span>|<span data-ttu-id="863b0-118">宛先 URL の宛先ドメイン部分。</span><span class="sxs-lookup"><span data-stu-id="863b0-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="863b0-119">(' www.contoso.com ' など)。</span><span class="sxs-lookup"><span data-stu-id="863b0-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="863b0-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="863b0-120">destinationPort</span></span>|<span data-ttu-id="863b0-121">String</span><span class="sxs-lookup"><span data-stu-id="863b0-121">String</span></span>|<span data-ttu-id="863b0-122">宛先ポート (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="863b0-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="863b0-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="863b0-123">destinationUrl</span></span>|<span data-ttu-id="863b0-124">String</span><span class="sxs-lookup"><span data-stu-id="863b0-124">String</span></span>|<span data-ttu-id="863b0-125">ネットワーク接続 URL/URI 文字列。パラメーターを除外します。</span><span class="sxs-lookup"><span data-stu-id="863b0-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="863b0-126">(' www.contoso.com/products/default.html ' など)</span><span class="sxs-lookup"><span data-stu-id="863b0-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="863b0-127">direction</span><span class="sxs-lookup"><span data-stu-id="863b0-127">direction</span></span>|<span data-ttu-id="863b0-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="863b0-128">connectionDirection</span></span>|<span data-ttu-id="863b0-129">ネットワーク接続の方向。</span><span class="sxs-lookup"><span data-stu-id="863b0-129">Network connection direction.</span></span> <span data-ttu-id="863b0-130">可能な値は、`unknown`、`inbound`、`outbound` です。</span><span class="sxs-lookup"><span data-stu-id="863b0-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="863b0-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="863b0-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="863b0-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="863b0-132">DateTimeOffset</span></span>|<span data-ttu-id="863b0-133">宛先ドメインが登録された日付。</span><span class="sxs-lookup"><span data-stu-id="863b0-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="863b0-134">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="863b0-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="863b0-135">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="863b0-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="863b0-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="863b0-136">localDnsName</span></span>|<span data-ttu-id="863b0-137">String</span><span class="sxs-lookup"><span data-stu-id="863b0-137">String</span></span>|<span data-ttu-id="863b0-138">ホストのローカル DNS キャッシュに表示されるローカル DNS 名解決方法 (たとえば、' hosts ' ファイルが改ざんされた場合)。</span><span class="sxs-lookup"><span data-stu-id="863b0-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="863b0-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="863b0-139">natDestinationAddress</span></span>|<span data-ttu-id="863b0-140">String</span><span class="sxs-lookup"><span data-stu-id="863b0-140">String</span></span>|<span data-ttu-id="863b0-141">ネットワークアドレス変換先 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="863b0-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="863b0-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="863b0-142">natDestinationPort</span></span>|<span data-ttu-id="863b0-143">String</span><span class="sxs-lookup"><span data-stu-id="863b0-143">String</span></span>|<span data-ttu-id="863b0-144">ネットワークアドレス変換先ポート。</span><span class="sxs-lookup"><span data-stu-id="863b0-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="863b0-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="863b0-145">natSourceAddress</span></span>|<span data-ttu-id="863b0-146">String</span><span class="sxs-lookup"><span data-stu-id="863b0-146">String</span></span>|<span data-ttu-id="863b0-147">ネットワークアドレス変換の送信元 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="863b0-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="863b0-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="863b0-148">natSourcePort</span></span>|<span data-ttu-id="863b0-149">String</span><span class="sxs-lookup"><span data-stu-id="863b0-149">String</span></span>|<span data-ttu-id="863b0-150">ネットワークアドレス変換元ポート。</span><span class="sxs-lookup"><span data-stu-id="863b0-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="863b0-151">プロトコール</span><span class="sxs-lookup"><span data-stu-id="863b0-151">protocol</span></span>|<span data-ttu-id="863b0-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="863b0-152">securityNetworkProtocol</span></span>|<span data-ttu-id="863b0-153">ネットワークプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-153">Network protocol.</span></span> <span data-ttu-id="863b0-154">可能な値: `unknown`、 `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader`、、、、、、、、、、、、 `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="863b0-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="863b0-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="863b0-155">riskScore</span></span>|<span data-ttu-id="863b0-156">String</span><span class="sxs-lookup"><span data-stu-id="863b0-156">String</span></span>|<span data-ttu-id="863b0-157">プロバイダーが生成/計算したネットワーク接続のリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="863b0-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="863b0-158">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="863b0-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="863b0-159">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="863b0-159">sourceAddress</span></span>|<span data-ttu-id="863b0-160">String</span><span class="sxs-lookup"><span data-stu-id="863b0-160">String</span></span>|<span data-ttu-id="863b0-161">ソース (起点) IP アドレス (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="863b0-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="863b0-162">sourcePort</span><span class="sxs-lookup"><span data-stu-id="863b0-162">sourcePort</span></span>|<span data-ttu-id="863b0-163">String</span><span class="sxs-lookup"><span data-stu-id="863b0-163">String</span></span>|<span data-ttu-id="863b0-164">ソース (起点) IP ポート (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="863b0-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="863b0-165">status</span><span class="sxs-lookup"><span data-stu-id="863b0-165">status</span></span>|<span data-ttu-id="863b0-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="863b0-166">connectionStatus</span></span>|<span data-ttu-id="863b0-167">ネットワーク接続の状態。</span><span class="sxs-lookup"><span data-stu-id="863b0-167">Network connection status.</span></span> <span data-ttu-id="863b0-168">可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="863b0-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="863b0-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="863b0-169">urlParameters</span></span>|<span data-ttu-id="863b0-170">String</span><span class="sxs-lookup"><span data-stu-id="863b0-170">String</span></span>|<span data-ttu-id="863b0-171">宛先 URL のパラメーター (サフィックス)。</span><span class="sxs-lookup"><span data-stu-id="863b0-171">Parameters (suffix) of the destination URL.</span></span>|

### <a name="securitynetworkprotocol-values"></a><span data-ttu-id="863b0-172">securityNetworkProtocol の値</span><span class="sxs-lookup"><span data-stu-id="863b0-172">securityNetworkProtocol values</span></span>

|<span data-ttu-id="863b0-173">メンバー</span><span class="sxs-lookup"><span data-stu-id="863b0-173">Member</span></span>|<span data-ttu-id="863b0-174">値</span><span class="sxs-lookup"><span data-stu-id="863b0-174">Value</span></span>|<span data-ttu-id="863b0-175">説明</span><span class="sxs-lookup"><span data-stu-id="863b0-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="863b0-176">不明</span><span class="sxs-lookup"><span data-stu-id="863b0-176">unknown</span></span>|<span data-ttu-id="863b0-177">-1</span><span class="sxs-lookup"><span data-stu-id="863b0-177">-1</span></span>|<span data-ttu-id="863b0-178">不明なプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-178">Unknown protocol.</span></span>|
|<span data-ttu-id="863b0-179">ip</span><span class="sxs-lookup"><span data-stu-id="863b0-179">ip</span></span>|<span data-ttu-id="863b0-180">.0</span><span class="sxs-lookup"><span data-stu-id="863b0-180">0</span></span>|<span data-ttu-id="863b0-181">インターネットプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-181">Internet Protocol.</span></span>|
|<span data-ttu-id="863b0-182">パケット</span><span class="sxs-lookup"><span data-stu-id="863b0-182">icmp</span></span>|<span data-ttu-id="863b0-183">1-d</span><span class="sxs-lookup"><span data-stu-id="863b0-183">1</span></span>| <span data-ttu-id="863b0-184">インターネットコントロールメッセージプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-184">Internet Control Message Protocol.</span></span>|
|<span data-ttu-id="863b0-185">igmp</span><span class="sxs-lookup"><span data-stu-id="863b0-185">igmp</span></span>|<span data-ttu-id="863b0-186">pbm-2</span><span class="sxs-lookup"><span data-stu-id="863b0-186">2</span></span>| <span data-ttu-id="863b0-187">インターネットグループ管理プロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-187">Internet Group Management Protocol.</span></span>|
|<span data-ttu-id="863b0-188">ggp</span><span class="sxs-lookup"><span data-stu-id="863b0-188">ggp</span></span>|<span data-ttu-id="863b0-189">1/3</span><span class="sxs-lookup"><span data-stu-id="863b0-189">3</span></span>| <span data-ttu-id="863b0-190">ゲートウェイからゲートウェイへのプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-190">Gateway To Gateway Protocol.</span></span>|
|<span data-ttu-id="863b0-191">ipv4</span><span class="sxs-lookup"><span data-stu-id="863b0-191">ipv4</span></span>|<span data-ttu-id="863b0-192">2/4</span><span class="sxs-lookup"><span data-stu-id="863b0-192">4</span></span>| <span data-ttu-id="863b0-193">インターネットプロトコルバージョン4。</span><span class="sxs-lookup"><span data-stu-id="863b0-193">Internet Protocol version 4.</span></span>|
|<span data-ttu-id="863b0-194">tcp</span><span class="sxs-lookup"><span data-stu-id="863b0-194">tcp</span></span>|<span data-ttu-id="863b0-195">シックス</span><span class="sxs-lookup"><span data-stu-id="863b0-195">6</span></span>| <span data-ttu-id="863b0-196">伝送制御プロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-196">Transmission Control Protocol.</span></span>|
|<span data-ttu-id="863b0-197">.pup</span><span class="sxs-lookup"><span data-stu-id="863b0-197">pup</span></span>|<span data-ttu-id="863b0-198">個</span><span class="sxs-lookup"><span data-stu-id="863b0-198">12</span></span>| <span data-ttu-id="863b0-199">PARC ユニバーサルパケットプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-199">PARC Universal Packet Protocol.</span></span>|
|<span data-ttu-id="863b0-200">受信</span><span class="sxs-lookup"><span data-stu-id="863b0-200">udp</span></span>|<span data-ttu-id="863b0-201">インチ</span><span class="sxs-lookup"><span data-stu-id="863b0-201">17</span></span>| <span data-ttu-id="863b0-202">ユーザーデータグラムプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-202">User Datagram Protocol.</span></span>|
|<span data-ttu-id="863b0-203">idp</span><span class="sxs-lookup"><span data-stu-id="863b0-203">idp</span></span>|<span data-ttu-id="863b0-204">×</span><span class="sxs-lookup"><span data-stu-id="863b0-204">22</span></span>| <span data-ttu-id="863b0-205">インターネットデータグラムプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-205">Internet Datagram Protocol.</span></span>|
|<span data-ttu-id="863b0-206">ipv6</span><span class="sxs-lookup"><span data-stu-id="863b0-206">ipv6</span></span>|<span data-ttu-id="863b0-207">41</span><span class="sxs-lookup"><span data-stu-id="863b0-207">41</span></span>| <span data-ttu-id="863b0-208">インターネットプロトコルバージョン 6 (ipv6)。</span><span class="sxs-lookup"><span data-stu-id="863b0-208">Internet Protocol version 6 (ipv6).</span></span>|
|<span data-ttu-id="863b0-209">ipv6RoutingHeader</span><span class="sxs-lookup"><span data-stu-id="863b0-209">ipv6RoutingHeader</span></span>|<span data-ttu-id="863b0-210">43</span><span class="sxs-lookup"><span data-stu-id="863b0-210">43</span></span>| <span data-ttu-id="863b0-211">ipv6 ルーティングヘッダー。</span><span class="sxs-lookup"><span data-stu-id="863b0-211">ipv6 Routing header.</span></span>|
|<span data-ttu-id="863b0-212">ipv6FragmentHeader</span><span class="sxs-lookup"><span data-stu-id="863b0-212">ipv6FragmentHeader</span></span>|<span data-ttu-id="863b0-213">44</span><span class="sxs-lookup"><span data-stu-id="863b0-213">44</span></span>| <span data-ttu-id="863b0-214">ipv6 フラグメントヘッダー。</span><span class="sxs-lookup"><span data-stu-id="863b0-214">ipv6 Fragment header.</span></span>|
|<span data-ttu-id="863b0-215">ipSecEncapsulatingSecurityPayload</span><span class="sxs-lookup"><span data-stu-id="863b0-215">ipSecEncapsulatingSecurityPayload</span></span>|<span data-ttu-id="863b0-216">50</span><span class="sxs-lookup"><span data-stu-id="863b0-216">50</span></span>| <span data-ttu-id="863b0-217">ipv6 カプセル化セキュリティペイロードヘッダー。</span><span class="sxs-lookup"><span data-stu-id="863b0-217">ipv6 Encapsulating Security Payload header.</span></span>|
|<span data-ttu-id="863b0-218">ipSecAuthenticationHeader</span><span class="sxs-lookup"><span data-stu-id="863b0-218">ipSecAuthenticationHeader</span></span>|<span data-ttu-id="863b0-219">51</span><span class="sxs-lookup"><span data-stu-id="863b0-219">51</span></span>| <span data-ttu-id="863b0-220">ipv6 認証ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="863b0-220">ipv6 Authentication header.</span></span>|
|<span data-ttu-id="863b0-221">過大</span><span class="sxs-lookup"><span data-stu-id="863b0-221">icmpV6</span></span>|<span data-ttu-id="863b0-222">58</span><span class="sxs-lookup"><span data-stu-id="863b0-222">58</span></span>| <span data-ttu-id="863b0-223">Ipv6 のインターネット制御メッセージプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-223">Internet Control Message Protocol for ipv6.</span></span>|
|<span data-ttu-id="863b0-224">ipv6NoNextHeader</span><span class="sxs-lookup"><span data-stu-id="863b0-224">ipv6NoNextHeader</span></span>|<span data-ttu-id="863b0-225">59</span><span class="sxs-lookup"><span data-stu-id="863b0-225">59</span></span>| <span data-ttu-id="863b0-226">ipv6 の次のヘッダーはありません。</span><span class="sxs-lookup"><span data-stu-id="863b0-226">ipv6 No next header.</span></span>|
|<span data-ttu-id="863b0-227">ipv6DestinationOptions</span><span class="sxs-lookup"><span data-stu-id="863b0-227">ipv6DestinationOptions</span></span>|<span data-ttu-id="863b0-228">60</span><span class="sxs-lookup"><span data-stu-id="863b0-228">60</span></span>| <span data-ttu-id="863b0-229">ipv6 宛先オプションヘッダー。</span><span class="sxs-lookup"><span data-stu-id="863b0-229">ipv6 Destination Options header.</span></span>|
|<span data-ttu-id="863b0-230">目</span><span class="sxs-lookup"><span data-stu-id="863b0-230">nd</span></span>|<span data-ttu-id="863b0-231">77</span><span class="sxs-lookup"><span data-stu-id="863b0-231">77</span></span>| <span data-ttu-id="863b0-232">ネットディスクプロトコル (非公式)。</span><span class="sxs-lookup"><span data-stu-id="863b0-232">Net Disk Protocol (unofficial).</span></span>|
|<span data-ttu-id="863b0-233">時</span><span class="sxs-lookup"><span data-stu-id="863b0-233">raw</span></span>|<span data-ttu-id="863b0-234">255</span><span class="sxs-lookup"><span data-stu-id="863b0-234">255</span></span>| <span data-ttu-id="863b0-235">生の IP パケットプロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-235">Raw IP packet protocol.</span></span>|
|<span data-ttu-id="863b0-236">ipx</span><span class="sxs-lookup"><span data-stu-id="863b0-236">ipx</span></span>|<span data-ttu-id="863b0-237">1000</span><span class="sxs-lookup"><span data-stu-id="863b0-237">1000</span></span>| <span data-ttu-id="863b0-238">インターネットパケット交換プロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-238">Internet Packet Exchange Protocol.</span></span>|
|<span data-ttu-id="863b0-239">spx</span><span class="sxs-lookup"><span data-stu-id="863b0-239">spx</span></span>|<span data-ttu-id="863b0-240">1256</span><span class="sxs-lookup"><span data-stu-id="863b0-240">1256</span></span>| <span data-ttu-id="863b0-241">順序付きパケット交換プロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-241">Sequenced Packet Exchange protocol.</span></span>|
|<span data-ttu-id="863b0-242">spxII</span><span class="sxs-lookup"><span data-stu-id="863b0-242">spxII</span></span>|<span data-ttu-id="863b0-243">1257</span><span class="sxs-lookup"><span data-stu-id="863b0-243">1257</span></span>| <span data-ttu-id="863b0-244">シーケンス付きパケット交換バージョン2プロトコル。</span><span class="sxs-lookup"><span data-stu-id="863b0-244">Sequenced Packet Exchange version 2 protocol.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="863b0-245">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="863b0-245">JSON representation</span></span>

<span data-ttu-id="863b0-246">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="863b0-246">The following is a JSON representation of the resource.</span></span>

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
  "direction": "String",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "string",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "String",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
