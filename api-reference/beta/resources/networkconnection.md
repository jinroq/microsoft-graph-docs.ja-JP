---
title: networkConnection リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: ce7de8d5a0f63c4d924e8092e4e9e05f984ec335
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570723"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="9a0b8-104">networkConnection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a0b8-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a0b8-105">通知に関連するネットワーク接続に関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="9a0b8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a0b8-106">Properties</span></span>

| <span data-ttu-id="9a0b8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a0b8-107">Property</span></span>   | <span data-ttu-id="9a0b8-108">型</span><span class="sxs-lookup"><span data-stu-id="9a0b8-108">Type</span></span>|<span data-ttu-id="9a0b8-109">説明</span><span class="sxs-lookup"><span data-stu-id="9a0b8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a0b8-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="9a0b8-110">applicationName</span></span>|<span data-ttu-id="9a0b8-111">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-111">String</span></span>|<span data-ttu-id="9a0b8-112">ネットワーク接続を管理しているアプリケーションの名前 (例: Facebook、SMTP など)。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="9a0b8-113">destinationaddress</span><span class="sxs-lookup"><span data-stu-id="9a0b8-113">destinationAddress</span></span>|<span data-ttu-id="9a0b8-114">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-114">String</span></span>|<span data-ttu-id="9a0b8-115">宛先 IP アドレス (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="9a0b8-116">destinationdomain</span><span class="sxs-lookup"><span data-stu-id="9a0b8-116">destinationDomain</span></span>|<span data-ttu-id="9a0b8-117">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-117">String</span></span>|<span data-ttu-id="9a0b8-118">宛先 URL の宛先ドメイン部分。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="9a0b8-119">(' www.contoso.com ' など)。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="9a0b8-120">destinationport</span><span class="sxs-lookup"><span data-stu-id="9a0b8-120">destinationPort</span></span>|<span data-ttu-id="9a0b8-121">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-121">String</span></span>|<span data-ttu-id="9a0b8-122">宛先ポート (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="9a0b8-123">destinationurl</span><span class="sxs-lookup"><span data-stu-id="9a0b8-123">destinationUrl</span></span>|<span data-ttu-id="9a0b8-124">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-124">String</span></span>|<span data-ttu-id="9a0b8-125">ネットワーク接続 URL/URI 文字列。パラメーターを除外します。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="9a0b8-126">(' www.contoso.com/products/default.html ' など)</span><span class="sxs-lookup"><span data-stu-id="9a0b8-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="9a0b8-127">direction</span><span class="sxs-lookup"><span data-stu-id="9a0b8-127">direction</span></span>|<span data-ttu-id="9a0b8-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="9a0b8-128">connectionDirection</span></span>|<span data-ttu-id="9a0b8-129">ネットワーク接続の方向。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-129">Network connection direction.</span></span> <span data-ttu-id="9a0b8-130">可能な値は `unknown`、`inbound`、`outbound` です。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="9a0b8-131">domainregistereddatetime</span><span class="sxs-lookup"><span data-stu-id="9a0b8-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="9a0b8-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a0b8-132">DateTimeOffset</span></span>|<span data-ttu-id="9a0b8-133">宛先ドメインが登録された日付。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="9a0b8-134">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a0b8-135">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9a0b8-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a0b8-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="9a0b8-136">localDnsName</span></span>|<span data-ttu-id="9a0b8-137">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-137">String</span></span>|<span data-ttu-id="9a0b8-138">ホストのローカル dns キャッシュに表示されるローカル dns 名解決方法 (たとえば、' hosts ' ファイルが改ざんされた場合)。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="9a0b8-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="9a0b8-139">natDestinationAddress</span></span>|<span data-ttu-id="9a0b8-140">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-140">String</span></span>|<span data-ttu-id="9a0b8-141">ネットワークアドレス変換先 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="9a0b8-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="9a0b8-142">natDestinationPort</span></span>|<span data-ttu-id="9a0b8-143">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-143">String</span></span>|<span data-ttu-id="9a0b8-144">ネットワークアドレス変換先ポート。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="9a0b8-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="9a0b8-145">natSourceAddress</span></span>|<span data-ttu-id="9a0b8-146">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-146">String</span></span>|<span data-ttu-id="9a0b8-147">ネットワークアドレス変換の送信元 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="9a0b8-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="9a0b8-148">natSourcePort</span></span>|<span data-ttu-id="9a0b8-149">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-149">String</span></span>|<span data-ttu-id="9a0b8-150">ネットワークアドレス変換元ポート。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="9a0b8-151">プロトコール</span><span class="sxs-lookup"><span data-stu-id="9a0b8-151">protocol</span></span>|[<span data-ttu-id="9a0b8-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="9a0b8-152">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="9a0b8-153">ネットワークプロトコル。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-153">Network protocol.</span></span> <span data-ttu-id="9a0b8-154">可能な値: `unknown`、 `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader`、、、、、、、、、、、、 `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="9a0b8-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="9a0b8-155">riskScore</span></span>|<span data-ttu-id="9a0b8-156">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-156">String</span></span>|<span data-ttu-id="9a0b8-157">プロバイダーが生成/計算したネットワーク接続のリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="9a0b8-158">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="9a0b8-159">sourceaddress</span><span class="sxs-lookup"><span data-stu-id="9a0b8-159">sourceAddress</span></span>|<span data-ttu-id="9a0b8-160">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-160">String</span></span>|<span data-ttu-id="9a0b8-161">ソース (起点) IP アドレス (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="9a0b8-162">sourceport</span><span class="sxs-lookup"><span data-stu-id="9a0b8-162">sourcePort</span></span>|<span data-ttu-id="9a0b8-163">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-163">String</span></span>|<span data-ttu-id="9a0b8-164">ソース (起点) IP ポート (ネットワーク接続の場合)。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="9a0b8-165">status</span><span class="sxs-lookup"><span data-stu-id="9a0b8-165">status</span></span>|<span data-ttu-id="9a0b8-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="9a0b8-166">connectionStatus</span></span>|<span data-ttu-id="9a0b8-167">ネットワーク接続の状態。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-167">Network connection status.</span></span> <span data-ttu-id="9a0b8-168">可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="9a0b8-169">urlparameters</span><span class="sxs-lookup"><span data-stu-id="9a0b8-169">urlParameters</span></span>|<span data-ttu-id="9a0b8-170">String</span><span class="sxs-lookup"><span data-stu-id="9a0b8-170">String</span></span>|<span data-ttu-id="9a0b8-171">宛先 URL のパラメーター (サフィックス)。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a0b8-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a0b8-172">JSON representation</span></span>

<span data-ttu-id="9a0b8-173">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a0b8-173">The following is a JSON representation of the resource.</span></span>

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
