---
title: ネットワーク接続リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 6d28149854ed3157473b678db442ee3474e456c6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571920"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="24bd8-104">ネットワーク接続リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24bd8-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24bd8-105">アラートに関連するネットワーク接続に関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="24bd8-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="24bd8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24bd8-106">Properties</span></span>

| <span data-ttu-id="24bd8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24bd8-107">Property</span></span>   | <span data-ttu-id="24bd8-108">型</span><span class="sxs-lookup"><span data-stu-id="24bd8-108">Type</span></span>|<span data-ttu-id="24bd8-109">説明</span><span class="sxs-lookup"><span data-stu-id="24bd8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24bd8-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="24bd8-110">applicationName</span></span>|<span data-ttu-id="24bd8-111">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-111">String</span></span>|<span data-ttu-id="24bd8-112">ネットワーク接続 (たとえば、Facebook、SMTP など) を管理するアプリケーションの名前です。</span><span class="sxs-lookup"><span data-stu-id="24bd8-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="24bd8-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="24bd8-113">destinationAddress</span></span>|<span data-ttu-id="24bd8-114">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-114">String</span></span>|<span data-ttu-id="24bd8-115">宛先 IP アドレス (ネットワーク接続)。</span><span class="sxs-lookup"><span data-stu-id="24bd8-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="24bd8-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="24bd8-116">destinationDomain</span></span>|<span data-ttu-id="24bd8-117">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-117">String</span></span>|<span data-ttu-id="24bd8-118">リンク先の URL のリンク先のドメイン部分です。</span><span class="sxs-lookup"><span data-stu-id="24bd8-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="24bd8-119">(たとえば ' www.contoso.com')。</span><span class="sxs-lookup"><span data-stu-id="24bd8-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="24bd8-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="24bd8-120">destinationPort</span></span>|<span data-ttu-id="24bd8-121">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-121">String</span></span>|<span data-ttu-id="24bd8-122">宛先ポート (ネットワーク接続)。</span><span class="sxs-lookup"><span data-stu-id="24bd8-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="24bd8-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="24bd8-123">destinationUrl</span></span>|<span data-ttu-id="24bd8-124">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-124">String</span></span>|<span data-ttu-id="24bd8-125">ネットワークの接続の URL または URI 文字列のパラメーターを除外します。</span><span class="sxs-lookup"><span data-stu-id="24bd8-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="24bd8-126">(たとえば ' www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="24bd8-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="24bd8-127">方向</span><span class="sxs-lookup"><span data-stu-id="24bd8-127">direction</span></span>|<span data-ttu-id="24bd8-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="24bd8-128">connectionDirection</span></span>|<span data-ttu-id="24bd8-129">ネットワーク接続の方向です。</span><span class="sxs-lookup"><span data-stu-id="24bd8-129">Network connection direction.</span></span> <span data-ttu-id="24bd8-130">可能な値は、`unknown`、`inbound`、`outbound` です。</span><span class="sxs-lookup"><span data-stu-id="24bd8-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="24bd8-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="24bd8-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="24bd8-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24bd8-132">DateTimeOffset</span></span>|<span data-ttu-id="24bd8-133">移行先のドメインが登録された日付です。</span><span class="sxs-lookup"><span data-stu-id="24bd8-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="24bd8-134">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="24bd8-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24bd8-135">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="24bd8-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="24bd8-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="24bd8-136">localDnsName</span></span>|<span data-ttu-id="24bd8-137">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-137">String</span></span>|<span data-ttu-id="24bd8-138">ローカル DNS 名前解決などの場合に 'ホスト' ファイルが改ざんされて)、ホストのローカル DNS キャッシュに表示されています。</span><span class="sxs-lookup"><span data-stu-id="24bd8-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="24bd8-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="24bd8-139">natDestinationAddress</span></span>|<span data-ttu-id="24bd8-140">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-140">String</span></span>|<span data-ttu-id="24bd8-141">ネットワーク アドレス変換の宛先 IP アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="24bd8-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="24bd8-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="24bd8-142">natDestinationPort</span></span>|<span data-ttu-id="24bd8-143">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-143">String</span></span>|<span data-ttu-id="24bd8-144">ネットワーク アドレス変換の送信先のポートを示します。</span><span class="sxs-lookup"><span data-stu-id="24bd8-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="24bd8-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="24bd8-145">natSourceAddress</span></span>|<span data-ttu-id="24bd8-146">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-146">String</span></span>|<span data-ttu-id="24bd8-147">ネットワーク アドレス変換の送信元 IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="24bd8-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="24bd8-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="24bd8-148">natSourcePort</span></span>|<span data-ttu-id="24bd8-149">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-149">String</span></span>|<span data-ttu-id="24bd8-150">ネットワーク アドレス変換のソース ポートです。</span><span class="sxs-lookup"><span data-stu-id="24bd8-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="24bd8-151">protocol</span><span class="sxs-lookup"><span data-stu-id="24bd8-151">protocol</span></span>| <span data-ttu-id="24bd8-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="24bd8-152">securityNetworkProtocol</span></span> |<span data-ttu-id="24bd8-153">ネットワーク プロトコルです。</span><span class="sxs-lookup"><span data-stu-id="24bd8-153">Network protocol.</span></span> <span data-ttu-id="24bd8-154">使用可能な値: `unknown`、 `ip`、 `icmp`、 `igmp`、 `ggp`、 `ipv4`、 `tcp`、 `pup`、 `udp`、 `idp`、 `ipv6`、 `ipv6RoutingHeader`、 `ipv6FragmentHeader`、 `ipSecEncapsulatingSecurityPayload`、 `ipSecAuthenticationHeader`、 `icmpV6`、 `ipv6NoNextHeader`、 `ipv6DestinationOptions`、 `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="24bd8-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="24bd8-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="24bd8-155">riskScore</span></span>|<span data-ttu-id="24bd8-156">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-156">String</span></span>|<span data-ttu-id="24bd8-157">プロバイダー生成された計算されるスコアのネットワーク接続の可能性があります。</span><span class="sxs-lookup"><span data-stu-id="24bd8-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="24bd8-158">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="24bd8-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="24bd8-159">発信元アドレス</span><span class="sxs-lookup"><span data-stu-id="24bd8-159">sourceAddress</span></span>|<span data-ttu-id="24bd8-160">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-160">String</span></span>|<span data-ttu-id="24bd8-161">(ネットワーク接続) の IP アドレスをソース (つまり原点)。</span><span class="sxs-lookup"><span data-stu-id="24bd8-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="24bd8-162">sourcePort</span><span class="sxs-lookup"><span data-stu-id="24bd8-162">sourcePort</span></span>|<span data-ttu-id="24bd8-163">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-163">String</span></span>|<span data-ttu-id="24bd8-164">(ネットワーク接続) の IP ポートをソース (つまり原点)。</span><span class="sxs-lookup"><span data-stu-id="24bd8-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="24bd8-165">status</span><span class="sxs-lookup"><span data-stu-id="24bd8-165">status</span></span>|<span data-ttu-id="24bd8-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="24bd8-166">connectionStatus</span></span>|<span data-ttu-id="24bd8-167">ネットワーク接続の状態です。</span><span class="sxs-lookup"><span data-stu-id="24bd8-167">Network connection status.</span></span> <span data-ttu-id="24bd8-168">可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="24bd8-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="24bd8-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="24bd8-169">urlParameters</span></span>|<span data-ttu-id="24bd8-170">String</span><span class="sxs-lookup"><span data-stu-id="24bd8-170">String</span></span>|<span data-ttu-id="24bd8-171">リンク先の URL のパラメーター (サフィックス) にします。</span><span class="sxs-lookup"><span data-stu-id="24bd8-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24bd8-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24bd8-172">JSON representation</span></span>

<span data-ttu-id="24bd8-173">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="24bd8-173">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/networkconnection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
