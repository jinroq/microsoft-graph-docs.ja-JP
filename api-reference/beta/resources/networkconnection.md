---
title: networkConnection リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 94bf27265f591d32c01e7043d3a10468a924d78a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342199"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="cb188-104">networkConnection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb188-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb188-105">通知に関連するネットワーク接続に関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="cb188-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="cb188-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb188-106">Properties</span></span>

| <span data-ttu-id="cb188-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb188-107">Property</span></span>   | <span data-ttu-id="cb188-108">型</span><span class="sxs-lookup"><span data-stu-id="cb188-108">Type</span></span>|<span data-ttu-id="cb188-109">説明</span><span class="sxs-lookup"><span data-stu-id="cb188-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb188-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="cb188-110">applicationName</span></span>|<span data-ttu-id="cb188-111">String</span><span class="sxs-lookup"><span data-stu-id="cb188-111">String</span></span>|<span data-ttu-id="cb188-112">ネットワーク接続を管理しているアプリケーションの名前 (例: Facebook、SMTP など)。</span><span class="sxs-lookup"><span data-stu-id="cb188-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="cb188-113">destinationaddress</span><span class="sxs-lookup"><span data-stu-id="cb188-113">destinationAddress</span></span>|<span data-ttu-id="cb188-114">String</span><span class="sxs-lookup"><span data-stu-id="cb188-114">String</span></span>|<span data-ttu-id="cb188-115">宛先 IP アドレス (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="cb188-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="cb188-116">destinationdomain</span><span class="sxs-lookup"><span data-stu-id="cb188-116">destinationDomain</span></span>|<span data-ttu-id="cb188-117">String</span><span class="sxs-lookup"><span data-stu-id="cb188-117">String</span></span>|<span data-ttu-id="cb188-118">宛先 URL の宛先ドメイン部分。</span><span class="sxs-lookup"><span data-stu-id="cb188-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="cb188-119">(' www.contoso.com ' など)。</span><span class="sxs-lookup"><span data-stu-id="cb188-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="cb188-120">destinationport</span><span class="sxs-lookup"><span data-stu-id="cb188-120">destinationPort</span></span>|<span data-ttu-id="cb188-121">String</span><span class="sxs-lookup"><span data-stu-id="cb188-121">String</span></span>|<span data-ttu-id="cb188-122">宛先ポート (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="cb188-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="cb188-123">destinationurl</span><span class="sxs-lookup"><span data-stu-id="cb188-123">destinationUrl</span></span>|<span data-ttu-id="cb188-124">String</span><span class="sxs-lookup"><span data-stu-id="cb188-124">String</span></span>|<span data-ttu-id="cb188-125">ネットワーク接続 URL/URI 文字列。パラメーターを除外します。</span><span class="sxs-lookup"><span data-stu-id="cb188-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="cb188-126">(' www.contoso.com/products/default.html ' など)</span><span class="sxs-lookup"><span data-stu-id="cb188-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="cb188-127">direction</span><span class="sxs-lookup"><span data-stu-id="cb188-127">direction</span></span>|<span data-ttu-id="cb188-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="cb188-128">connectionDirection</span></span>|<span data-ttu-id="cb188-129">ネットワーク接続の方向。</span><span class="sxs-lookup"><span data-stu-id="cb188-129">Network connection direction.</span></span> <span data-ttu-id="cb188-130">可能な値は、`unknown`、`inbound`、`outbound` です。</span><span class="sxs-lookup"><span data-stu-id="cb188-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="cb188-131">domainregistereddatetime</span><span class="sxs-lookup"><span data-stu-id="cb188-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="cb188-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb188-132">DateTimeOffset</span></span>|<span data-ttu-id="cb188-133">宛先ドメインが登録された日付。</span><span class="sxs-lookup"><span data-stu-id="cb188-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="cb188-134">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="cb188-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cb188-135">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cb188-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cb188-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="cb188-136">localDnsName</span></span>|<span data-ttu-id="cb188-137">String</span><span class="sxs-lookup"><span data-stu-id="cb188-137">String</span></span>|<span data-ttu-id="cb188-138">ホストのローカル dns キャッシュに表示されるローカル dns 名解決方法 (たとえば、' hosts ' ファイルが改ざんされた場合)。</span><span class="sxs-lookup"><span data-stu-id="cb188-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="cb188-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="cb188-139">natDestinationAddress</span></span>|<span data-ttu-id="cb188-140">String</span><span class="sxs-lookup"><span data-stu-id="cb188-140">String</span></span>|<span data-ttu-id="cb188-141">ネットワークアドレス変換先 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="cb188-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="cb188-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="cb188-142">natDestinationPort</span></span>|<span data-ttu-id="cb188-143">String</span><span class="sxs-lookup"><span data-stu-id="cb188-143">String</span></span>|<span data-ttu-id="cb188-144">ネットワークアドレス変換先ポート。</span><span class="sxs-lookup"><span data-stu-id="cb188-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="cb188-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="cb188-145">natSourceAddress</span></span>|<span data-ttu-id="cb188-146">String</span><span class="sxs-lookup"><span data-stu-id="cb188-146">String</span></span>|<span data-ttu-id="cb188-147">ネットワークアドレス変換の送信元 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="cb188-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="cb188-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="cb188-148">natSourcePort</span></span>|<span data-ttu-id="cb188-149">String</span><span class="sxs-lookup"><span data-stu-id="cb188-149">String</span></span>|<span data-ttu-id="cb188-150">ネットワークアドレス変換元ポート。</span><span class="sxs-lookup"><span data-stu-id="cb188-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="cb188-151">プロトコール</span><span class="sxs-lookup"><span data-stu-id="cb188-151">protocol</span></span>|<span data-ttu-id="cb188-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="cb188-152">securityNetworkProtocol</span></span>|<span data-ttu-id="cb188-153">ネットワークプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-153">Network protocol.</span></span> <span data-ttu-id="cb188-154">可能な値: `unknown`、 `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader`、、、、、、、、、、、、 `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="cb188-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="cb188-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="cb188-155">riskScore</span></span>|<span data-ttu-id="cb188-156">String</span><span class="sxs-lookup"><span data-stu-id="cb188-156">String</span></span>|<span data-ttu-id="cb188-157">プロバイダーが生成/計算したネットワーク接続のリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="cb188-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="cb188-158">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="cb188-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="cb188-159">sourceaddress</span><span class="sxs-lookup"><span data-stu-id="cb188-159">sourceAddress</span></span>|<span data-ttu-id="cb188-160">String</span><span class="sxs-lookup"><span data-stu-id="cb188-160">String</span></span>|<span data-ttu-id="cb188-161">ソース (起点) IP アドレス (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="cb188-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="cb188-162">sourceport</span><span class="sxs-lookup"><span data-stu-id="cb188-162">sourcePort</span></span>|<span data-ttu-id="cb188-163">String</span><span class="sxs-lookup"><span data-stu-id="cb188-163">String</span></span>|<span data-ttu-id="cb188-164">ソース (起点) IP ポート (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="cb188-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="cb188-165">status</span><span class="sxs-lookup"><span data-stu-id="cb188-165">status</span></span>|<span data-ttu-id="cb188-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="cb188-166">connectionStatus</span></span>|<span data-ttu-id="cb188-167">ネットワーク接続の状態。</span><span class="sxs-lookup"><span data-stu-id="cb188-167">Network connection status.</span></span> <span data-ttu-id="cb188-168">可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="cb188-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="cb188-169">urlparameters</span><span class="sxs-lookup"><span data-stu-id="cb188-169">urlParameters</span></span>|<span data-ttu-id="cb188-170">String</span><span class="sxs-lookup"><span data-stu-id="cb188-170">String</span></span>|<span data-ttu-id="cb188-171">宛先 URL のパラメーター (サフィックス)。</span><span class="sxs-lookup"><span data-stu-id="cb188-171">Parameters (suffix) of the destination URL.</span></span>|

### <a name="securitynetworkprotocol-values"></a><span data-ttu-id="cb188-172">securitynetworkprotocol の値</span><span class="sxs-lookup"><span data-stu-id="cb188-172">securityNetworkProtocol values</span></span>

|<span data-ttu-id="cb188-173">メンバー</span><span class="sxs-lookup"><span data-stu-id="cb188-173">Member</span></span>|<span data-ttu-id="cb188-174">値</span><span class="sxs-lookup"><span data-stu-id="cb188-174">Value</span></span>|<span data-ttu-id="cb188-175">説明</span><span class="sxs-lookup"><span data-stu-id="cb188-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb188-176">不明</span><span class="sxs-lookup"><span data-stu-id="cb188-176">unknown</span></span>|<span data-ttu-id="cb188-177">-1</span><span class="sxs-lookup"><span data-stu-id="cb188-177">-1</span></span>|<span data-ttu-id="cb188-178">不明なプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-178">Unknown protocol.</span></span>|
|<span data-ttu-id="cb188-179">ip</span><span class="sxs-lookup"><span data-stu-id="cb188-179">ip</span></span>|<span data-ttu-id="cb188-180">.0</span><span class="sxs-lookup"><span data-stu-id="cb188-180">0</span></span>|<span data-ttu-id="cb188-181">インターネットプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-181">Internet Protocol.</span></span>|
|<span data-ttu-id="cb188-182">パケット</span><span class="sxs-lookup"><span data-stu-id="cb188-182">icmp</span></span>|<span data-ttu-id="cb188-183">1-d</span><span class="sxs-lookup"><span data-stu-id="cb188-183">1</span></span>| <span data-ttu-id="cb188-184">インターネットコントロールメッセージプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-184">Internet Control Message Protocol.</span></span>|
|<span data-ttu-id="cb188-185">igmp</span><span class="sxs-lookup"><span data-stu-id="cb188-185">igmp</span></span>|<span data-ttu-id="cb188-186">pbm-2</span><span class="sxs-lookup"><span data-stu-id="cb188-186">2</span></span>| <span data-ttu-id="cb188-187">インターネットグループ管理プロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-187">Internet Group Management Protocol.</span></span>|
|<span data-ttu-id="cb188-188">ggp</span><span class="sxs-lookup"><span data-stu-id="cb188-188">ggp</span></span>|<span data-ttu-id="cb188-189">1/3</span><span class="sxs-lookup"><span data-stu-id="cb188-189">3</span></span>| <span data-ttu-id="cb188-190">ゲートウェイからゲートウェイへのプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-190">Gateway To Gateway Protocol.</span></span>|
|<span data-ttu-id="cb188-191">ipv4</span><span class="sxs-lookup"><span data-stu-id="cb188-191">ipv4</span></span>|<span data-ttu-id="cb188-192">2/4</span><span class="sxs-lookup"><span data-stu-id="cb188-192">4</span></span>| <span data-ttu-id="cb188-193">インターネットプロトコルバージョン4。</span><span class="sxs-lookup"><span data-stu-id="cb188-193">Internet Protocol version 4.</span></span>|
|<span data-ttu-id="cb188-194">tcp</span><span class="sxs-lookup"><span data-stu-id="cb188-194">tcp</span></span>|<span data-ttu-id="cb188-195">シックス</span><span class="sxs-lookup"><span data-stu-id="cb188-195">6</span></span>| <span data-ttu-id="cb188-196">伝送制御プロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-196">Transmission Control Protocol.</span></span>|
|<span data-ttu-id="cb188-197">.pup</span><span class="sxs-lookup"><span data-stu-id="cb188-197">pup</span></span>|<span data-ttu-id="cb188-198">12 </span><span class="sxs-lookup"><span data-stu-id="cb188-198">12</span></span>| <span data-ttu-id="cb188-199">parc ユニバーサルパケットプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-199">PARC Universal Packet Protocol.</span></span>|
|<span data-ttu-id="cb188-200">受信</span><span class="sxs-lookup"><span data-stu-id="cb188-200">udp</span></span>|<span data-ttu-id="cb188-201">17 </span><span class="sxs-lookup"><span data-stu-id="cb188-201">17</span></span>| <span data-ttu-id="cb188-202">ユーザーデータグラムプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-202">User Datagram Protocol.</span></span>|
|<span data-ttu-id="cb188-203">idp</span><span class="sxs-lookup"><span data-stu-id="cb188-203">idp</span></span>|<span data-ttu-id="cb188-204">×</span><span class="sxs-lookup"><span data-stu-id="cb188-204">22</span></span>| <span data-ttu-id="cb188-205">インターネットデータグラムプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-205">Internet Datagram Protocol.</span></span>|
|<span data-ttu-id="cb188-206">ipv6</span><span class="sxs-lookup"><span data-stu-id="cb188-206">ipv6</span></span>|<span data-ttu-id="cb188-207">41</span><span class="sxs-lookup"><span data-stu-id="cb188-207">41</span></span>| <span data-ttu-id="cb188-208">インターネットプロトコルバージョン 6 (ipv6)。</span><span class="sxs-lookup"><span data-stu-id="cb188-208">Internet Protocol version 6 (ipv6).</span></span>|
|<span data-ttu-id="cb188-209">ipv6RoutingHeader</span><span class="sxs-lookup"><span data-stu-id="cb188-209">ipv6RoutingHeader</span></span>|<span data-ttu-id="cb188-210">43</span><span class="sxs-lookup"><span data-stu-id="cb188-210">43</span></span>| <span data-ttu-id="cb188-211">ipv6 ルーティングヘッダー。</span><span class="sxs-lookup"><span data-stu-id="cb188-211">ipv6 Routing header.</span></span>|
|<span data-ttu-id="cb188-212">ipv6FragmentHeader</span><span class="sxs-lookup"><span data-stu-id="cb188-212">ipv6FragmentHeader</span></span>|<span data-ttu-id="cb188-213">44</span><span class="sxs-lookup"><span data-stu-id="cb188-213">44</span></span>| <span data-ttu-id="cb188-214">ipv6 フラグメントヘッダー。</span><span class="sxs-lookup"><span data-stu-id="cb188-214">ipv6 Fragment header.</span></span>|
|<span data-ttu-id="cb188-215">ipSecEncapsulatingSecurityPayload</span><span class="sxs-lookup"><span data-stu-id="cb188-215">ipSecEncapsulatingSecurityPayload</span></span>|<span data-ttu-id="cb188-216">50</span><span class="sxs-lookup"><span data-stu-id="cb188-216">50</span></span>| <span data-ttu-id="cb188-217">ipv6 カプセル化セキュリティペイロードヘッダー。</span><span class="sxs-lookup"><span data-stu-id="cb188-217">ipv6 Encapsulating Security Payload header.</span></span>|
|<span data-ttu-id="cb188-218">ipsecauthenticationheader</span><span class="sxs-lookup"><span data-stu-id="cb188-218">ipSecAuthenticationHeader</span></span>|<span data-ttu-id="cb188-219">51</span><span class="sxs-lookup"><span data-stu-id="cb188-219">51</span></span>| <span data-ttu-id="cb188-220">ipv6 認証ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="cb188-220">ipv6 Authentication header.</span></span>|
|<span data-ttu-id="cb188-221">過大</span><span class="sxs-lookup"><span data-stu-id="cb188-221">icmpV6</span></span>|<span data-ttu-id="cb188-222">58</span><span class="sxs-lookup"><span data-stu-id="cb188-222">58</span></span>| <span data-ttu-id="cb188-223">ipv6 のインターネット制御メッセージプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-223">Internet Control Message Protocol for ipv6.</span></span>|
|<span data-ttu-id="cb188-224">ipv6NoNextHeader</span><span class="sxs-lookup"><span data-stu-id="cb188-224">ipv6NoNextHeader</span></span>|<span data-ttu-id="cb188-225">59</span><span class="sxs-lookup"><span data-stu-id="cb188-225">59</span></span>| <span data-ttu-id="cb188-226">ipv6 の次のヘッダーはありません。</span><span class="sxs-lookup"><span data-stu-id="cb188-226">ipv6 No next header.</span></span>|
|<span data-ttu-id="cb188-227">ipv6DestinationOptions</span><span class="sxs-lookup"><span data-stu-id="cb188-227">ipv6DestinationOptions</span></span>|<span data-ttu-id="cb188-228">60</span><span class="sxs-lookup"><span data-stu-id="cb188-228">60</span></span>| <span data-ttu-id="cb188-229">ipv6 宛先オプションヘッダー。</span><span class="sxs-lookup"><span data-stu-id="cb188-229">ipv6 Destination Options header.</span></span>|
|<span data-ttu-id="cb188-230">目</span><span class="sxs-lookup"><span data-stu-id="cb188-230">nd</span></span>|<span data-ttu-id="cb188-231">77</span><span class="sxs-lookup"><span data-stu-id="cb188-231">77</span></span>| <span data-ttu-id="cb188-232">ネットディスクプロトコル (非公式)。</span><span class="sxs-lookup"><span data-stu-id="cb188-232">Net Disk Protocol (unofficial).</span></span>|
|<span data-ttu-id="cb188-233">時</span><span class="sxs-lookup"><span data-stu-id="cb188-233">raw</span></span>|<span data-ttu-id="cb188-234">255</span><span class="sxs-lookup"><span data-stu-id="cb188-234">255</span></span>| <span data-ttu-id="cb188-235">生の IP パケットプロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-235">Raw IP packet protocol.</span></span>|
|<span data-ttu-id="cb188-236">ipx</span><span class="sxs-lookup"><span data-stu-id="cb188-236">ipx</span></span>|<span data-ttu-id="cb188-237">1000</span><span class="sxs-lookup"><span data-stu-id="cb188-237">1000</span></span>| <span data-ttu-id="cb188-238">インターネットパケット交換プロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-238">Internet Packet Exchange Protocol.</span></span>|
|<span data-ttu-id="cb188-239">spx</span><span class="sxs-lookup"><span data-stu-id="cb188-239">spx</span></span>|<span data-ttu-id="cb188-240">1256</span><span class="sxs-lookup"><span data-stu-id="cb188-240">1256</span></span>| <span data-ttu-id="cb188-241">順序付きパケット交換プロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-241">Sequenced Packet Exchange protocol.</span></span>|
|<span data-ttu-id="cb188-242">spxii</span><span class="sxs-lookup"><span data-stu-id="cb188-242">spxII</span></span>|<span data-ttu-id="cb188-243">1257</span><span class="sxs-lookup"><span data-stu-id="cb188-243">1257</span></span>| <span data-ttu-id="cb188-244">シーケンス付きパケット交換バージョン2プロトコル。</span><span class="sxs-lookup"><span data-stu-id="cb188-244">Sequenced Packet Exchange version 2 protocol.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb188-245">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb188-245">JSON representation</span></span>

<span data-ttu-id="cb188-246">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb188-246">The following is a JSON representation of the resource.</span></span>

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
