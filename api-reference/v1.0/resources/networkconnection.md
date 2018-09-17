# <a name="networkconnection-resource-type"></a><span data-ttu-id="54f4f-101">ネットワーク接続リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54f4f-101">networkConnection resource type</span></span>

<span data-ttu-id="54f4f-102">アラートに関連するネットワーク接続に関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="54f4f-102">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="54f4f-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54f4f-103">Properties</span></span>

| <span data-ttu-id="54f4f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54f4f-104">Property</span></span>   | <span data-ttu-id="54f4f-105">型</span><span class="sxs-lookup"><span data-stu-id="54f4f-105">Type</span></span>|<span data-ttu-id="54f4f-106">説明</span><span class="sxs-lookup"><span data-stu-id="54f4f-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54f4f-107">applicationName</span><span class="sxs-lookup"><span data-stu-id="54f4f-107">applicationName</span></span>|<span data-ttu-id="54f4f-108">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-108">String</span></span>|<span data-ttu-id="54f4f-109">ネットワーク接続 (たとえば、Facebook、SMTP など) を管理するアプリケーションの名前です。</span><span class="sxs-lookup"><span data-stu-id="54f4f-109">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="54f4f-110">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="54f4f-110">destinationAddress</span></span>|<span data-ttu-id="54f4f-111">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-111">String</span></span>|<span data-ttu-id="54f4f-112">宛先 IP アドレス (ネットワーク接続)。</span><span class="sxs-lookup"><span data-stu-id="54f4f-112">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="54f4f-113">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="54f4f-113">destinationDomain</span></span>|<span data-ttu-id="54f4f-114">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-114">String</span></span>|<span data-ttu-id="54f4f-115">リンク先の URL のリンク先のドメイン部分です。</span><span class="sxs-lookup"><span data-stu-id="54f4f-115">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="54f4f-116">(例えば ' www.contoso.com')。</span><span class="sxs-lookup"><span data-stu-id="54f4f-116">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="54f4f-117">destinationPort</span><span class="sxs-lookup"><span data-stu-id="54f4f-117">destinationPort</span></span>|<span data-ttu-id="54f4f-118">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-118">String</span></span>|<span data-ttu-id="54f4f-119">宛先ポート (ネットワーク接続)。</span><span class="sxs-lookup"><span data-stu-id="54f4f-119">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="54f4f-120">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="54f4f-120">destinationUrl</span></span>|<span data-ttu-id="54f4f-121">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-121">String</span></span>|<span data-ttu-id="54f4f-122">ネットワークの接続の URL または URI 文字列のパラメーターを除外します。</span><span class="sxs-lookup"><span data-stu-id="54f4f-122">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="54f4f-123">(例えば ' www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="54f4f-123">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="54f4f-124">direction</span><span class="sxs-lookup"><span data-stu-id="54f4f-124">direction</span></span>|<span data-ttu-id="54f4f-125">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="54f4f-125">connectionDirection</span></span>|<span data-ttu-id="54f4f-126">ネットワーク接続の方向です。</span><span class="sxs-lookup"><span data-stu-id="54f4f-126">Network connection direction.</span></span> <span data-ttu-id="54f4f-127">可能な値は、`unknown`、`inbound`、`outbound` です。</span><span class="sxs-lookup"><span data-stu-id="54f4f-127">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="54f4f-128">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="54f4f-128">domainRegisteredDateTime</span></span>|<span data-ttu-id="54f4f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54f4f-129">DateTimeOffset</span></span>|<span data-ttu-id="54f4f-130">移行先のドメインが登録された日付です。</span><span class="sxs-lookup"><span data-stu-id="54f4f-130">Date when the destination domain was registered.</span></span> <span data-ttu-id="54f4f-131">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="54f4f-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="54f4f-132">例えば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="54f4f-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="54f4f-133">localDnsName</span><span class="sxs-lookup"><span data-stu-id="54f4f-133">localDnsName</span></span>|<span data-ttu-id="54f4f-134">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-134">String</span></span>|<span data-ttu-id="54f4f-135">ローカル DNS 名前解決などの場合に 'ホスト' ファイルが改ざんされて)、ホストのローカル DNS キャッシュに表示されています。</span><span class="sxs-lookup"><span data-stu-id="54f4f-135">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="54f4f-136">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="54f4f-136">natDestinationAddress</span></span>|<span data-ttu-id="54f4f-137">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-137">String</span></span>|<span data-ttu-id="54f4f-138">ネットワークアドレス変換の宛先 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="54f4f-138">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="54f4f-139">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="54f4f-139">natDestinationPort</span></span>|<span data-ttu-id="54f4f-140">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-140">String</span></span>|<span data-ttu-id="54f4f-141">ネットワーク アドレス変換の送信先のポート。</span><span class="sxs-lookup"><span data-stu-id="54f4f-141">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="54f4f-142">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="54f4f-142">natSourceAddress</span></span>|<span data-ttu-id="54f4f-143">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-143">String</span></span>|<span data-ttu-id="54f4f-144">ネットワーク アドレス変換の送信元 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="54f4f-144">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="54f4f-145">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="54f4f-145">natSourcePort</span></span>|<span data-ttu-id="54f4f-146">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-146">String</span></span>|<span data-ttu-id="54f4f-147">ネットワークアドレス変換のソースポート。</span><span class="sxs-lookup"><span data-stu-id="54f4f-147">Network Address Translation source port.</span></span>|
|<span data-ttu-id="54f4f-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="54f4f-148">protocol</span></span>|[<span data-ttu-id="54f4f-149">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="54f4f-149">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="54f4f-150">ネットワークプロトコル</span><span class="sxs-lookup"><span data-stu-id="54f4f-150">Network protocol analysis</span></span> <span data-ttu-id="54f4f-151">使用可能な値は: `unknown`、 `ip`、 `icmp`、 `igmp`、 `ggp`、 `ipv4`、 `tcp`、 `pup`、 `udp`、 `idp`、 `ipv6`、 `ipv6RoutingHeader`、 `ipv6FragmentHeader`、 `ipSecEncapsulatingSecurityPayload`、 `ipSecAuthenticationHeader`、 `icmpV6`、 `ipv6NoNextHeader`、 `ipv6DestinationOptions`、 `nd`, `raw`, `ipx`, `spx`, `spxII`です。</span><span class="sxs-lookup"><span data-stu-id="54f4f-151">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`.</span></span>|
|<span data-ttu-id="54f4f-152">riskScore</span><span class="sxs-lookup"><span data-stu-id="54f4f-152">riskScore</span></span>|<span data-ttu-id="54f4f-153">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-153">String</span></span>|<span data-ttu-id="54f4f-154">プロバイダーが生成または計算した、ネットワーク接続のリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="54f4f-154">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="54f4f-155">パーセンテージに相当する 0 - 1 の値の範囲を推奨します。</span><span class="sxs-lookup"><span data-stu-id="54f4f-155">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="54f4f-156">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="54f4f-156">sourceAddress</span></span>|<span data-ttu-id="54f4f-157">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-157">String</span></span>|<span data-ttu-id="54f4f-158">ソース (つまり原点)(ネットワーク接続の)  IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="54f4f-158">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="54f4f-159">sourcePort</span><span class="sxs-lookup"><span data-stu-id="54f4f-159">sourcePort</span></span>|<span data-ttu-id="54f4f-160">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-160">String</span></span>|<span data-ttu-id="54f4f-161">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-161">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="54f4f-162">状態</span><span class="sxs-lookup"><span data-stu-id="54f4f-162">status</span></span>|<span data-ttu-id="54f4f-163">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="54f4f-163">ConnectionStatus</span></span>|<span data-ttu-id="54f4f-164">ネットワーク接続の状態。</span><span class="sxs-lookup"><span data-stu-id="54f4f-164">Network connection status.</span></span> <span data-ttu-id="54f4f-165">可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="54f4f-165">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="54f4f-166">urlParameters</span><span class="sxs-lookup"><span data-stu-id="54f4f-166">urlParameters</span></span>|<span data-ttu-id="54f4f-167">文字列</span><span class="sxs-lookup"><span data-stu-id="54f4f-167">String</span></span>|<span data-ttu-id="54f4f-168">リンク先URLのパラメーター(サフィックス)。</span><span class="sxs-lookup"><span data-stu-id="54f4f-168">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54f4f-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54f4f-169">JSON representation</span></span>

<span data-ttu-id="54f4f-170">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="54f4f-170">The following is a JSON representation of the resource.</span></span>

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