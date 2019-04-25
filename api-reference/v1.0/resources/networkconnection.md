---
title: networkConnection リソースの種類
description: 通知に関連するネットワーク接続に関するステートフルな情報を含みます。
localization_priority: Normal
ms.openlocfilehash: 78ddcfd19d68b8dcd64c74a5beed6d1430f0ca38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580276"
---
# <a name="networkconnection-resource-type"></a>networkConnection リソースの種類

通知に関連するネットワーク接続に関するステートフルな情報を含みます。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|applicationName|String|ネットワーク接続を管理しているアプリケーションの名前 (例: Facebook、SMTP など)。|
|destinationaddress|String|宛先 IP アドレス (ネットワーク接続の場合)。|
|destinationdomain|String|宛先 URL の宛先ドメイン部分。 (' www.contoso.com ' など)。|
|destinationport|String|宛先ポート (ネットワーク接続の場合)。|
|destinationurl|String|ネットワーク接続 URL/URI 文字列。パラメーターを除外します。 (' www.contoso.com/products/default.html ' など)|
|direction|connectionDirection|ネットワーク接続の方向。 可能な値は `unknown`、`inbound`、`outbound` です。|
|domainregistereddatetime|DateTimeOffset|宛先ドメインが登録された日付。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|localDnsName|String|ホストのローカル dns キャッシュに表示されるローカル dns 名解決方法 (たとえば、' hosts ' ファイルが改ざんされた場合)。|
|natDestinationAddress|String|ネットワークアドレス変換先 IP アドレス。|
|natDestinationPort|String|ネットワークアドレス変換先ポート。|
|natSourceAddress|String|ネットワークアドレス変換の送信元 IP アドレス。|
|natSourcePort|String|ネットワークアドレス変換元ポート。|
|プロトコール|[securityNetworkProtocol](securitynetworkprotocol.md)|ネットワークプロトコル。 可能な値: `unknown`、 `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader`、、、、、、、、、、、、 `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd`, `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|String|プロバイダーが生成/計算したネットワーク接続のリスクスコア。 推奨値の範囲0-1。パーセンテージに相当します。|
|sourceaddress|String|ソース (起点) IP アドレス (ネットワーク接続の場合)。|
|sourceport|String|ソース (起点) IP ポート (ネットワーク接続の場合)。|
|status|connectionStatus|ネットワーク接続の状態。 可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。|
|urlparameters|String|宛先 URL のパラメーター (サフィックス)。|

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
