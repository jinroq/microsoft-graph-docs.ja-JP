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
# <a name="networkconnection-resource-type"></a>ネットワーク接続リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アラートに関連するネットワーク接続に関するステートフルな情報が含まれています。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|applicationName|String|ネットワーク接続 (たとえば、Facebook、SMTP など) を管理するアプリケーションの名前です。|
|destinationAddress|String|宛先 IP アドレス (ネットワーク接続)。|
|destinationDomain|String|リンク先の URL のリンク先のドメイン部分です。 (たとえば ' www.contoso.com')。|
|destinationPort|String|宛先ポート (ネットワーク接続)。|
|destinationUrl|String|ネットワークの接続の URL または URI 文字列のパラメーターを除外します。 (たとえば ' www.contoso.com/products/default.html')|
|方向|connectionDirection|ネットワーク接続の方向です。 可能な値は、`unknown`、`inbound`、`outbound` です。|
|domainRegisteredDateTime|DateTimeOffset|移行先のドメインが登録された日付です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|localDnsName|String|ローカル DNS 名前解決などの場合に 'ホスト' ファイルが改ざんされて)、ホストのローカル DNS キャッシュに表示されています。|
|natDestinationAddress|String|ネットワーク アドレス変換の宛先 IP アドレスを示します。|
|natDestinationPort|String|ネットワーク アドレス変換の送信先のポートを示します。|
|natSourceAddress|String|ネットワーク アドレス変換の送信元 IP アドレスです。|
|natSourcePort|String|ネットワーク アドレス変換のソース ポートです。|
|protocol|[securityNetworkProtocol](securitynetworkprotocolenumtype.md)|ネットワーク プロトコルです。 使用可能な値: `unknown`、 `ip`、 `icmp`、 `igmp`、 `ggp`、 `ipv4`、 `tcp`、 `pup`、 `udp`、 `idp`、 `ipv6`、 `ipv6RoutingHeader`、 `ipv6FragmentHeader`、 `ipSecEncapsulatingSecurityPayload`、 `ipSecAuthenticationHeader`、 `icmpV6`、 `ipv6NoNextHeader`、 `ipv6DestinationOptions`、 `nd`, `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|String|プロバイダー生成された計算されるスコアのネットワーク接続の可能性があります。 0 - 1 パーセントに相当する値の範囲をお勧めします。|
|発信元アドレス|String|(ネットワーク接続) の IP アドレスをソース (つまり原点)。|
|sourcePort|String|(ネットワーク接続) の IP ポートをソース (つまり原点)。|
|status|connectionStatus|ネットワーク接続の状態です。 可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。|
|urlParameters|String|リンク先の URL のパラメーター (サフィックス) にします。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

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
