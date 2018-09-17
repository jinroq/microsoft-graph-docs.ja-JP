# <a name="networkconnection-resource-type"></a>ネットワーク接続リソースの種類

アラートに関連するネットワーク接続に関するステートフルな情報が含まれています。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|applicationName|文字列|ネットワーク接続 (たとえば、Facebook、SMTP など) を管理するアプリケーションの名前です。|
|destinationAddress|文字列|宛先 IP アドレス (ネットワーク接続)。|
|destinationDomain|文字列|リンク先の URL のリンク先のドメイン部分です。 (例えば ' www.contoso.com')。|
|destinationPort|文字列|宛先ポート (ネットワーク接続)。|
|destinationUrl|文字列|ネットワークの接続の URL または URI 文字列のパラメーターを除外します。 (例えば ' www.contoso.com/products/default.html')|
|direction|connectionDirection|ネットワーク接続の方向です。 可能な値は、`unknown`、`inbound`、`outbound` です。|
|domainRegisteredDateTime|DateTimeOffset|移行先のドメインが登録された日付です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 例えば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`|
|localDnsName|文字列|ローカル DNS 名前解決などの場合に 'ホスト' ファイルが改ざんされて)、ホストのローカル DNS キャッシュに表示されています。|
|natDestinationAddress|文字列|ネットワークアドレス変換の宛先 IP アドレス。|
|natDestinationPort|文字列|ネットワーク アドレス変換の送信先のポート。|
|natSourceAddress|文字列|ネットワーク アドレス変換の送信元 IP アドレス。|
|natSourcePort|文字列|ネットワークアドレス変換のソースポート。|
|プロトコル|[securityNetworkProtocol](securitynetworkprotocol.md)|ネットワークプロトコル 使用可能な値は: `unknown`、 `ip`、 `icmp`、 `igmp`、 `ggp`、 `ipv4`、 `tcp`、 `pup`、 `udp`、 `idp`、 `ipv6`、 `ipv6RoutingHeader`、 `ipv6FragmentHeader`、 `ipSecEncapsulatingSecurityPayload`、 `ipSecAuthenticationHeader`、 `icmpV6`、 `ipv6NoNextHeader`、 `ipv6DestinationOptions`、 `nd`, `raw`, `ipx`, `spx`, `spxII`です。|
|riskScore|文字列|プロバイダーが生成または計算した、ネットワーク接続のリスクスコア。 パーセンテージに相当する 0 - 1 の値の範囲を推奨します。|
|sourceAddress|文字列|ソース (つまり原点)(ネットワーク接続の)  IP アドレス。|
|sourcePort|文字列|文字列|
|状態|ConnectionStatus|ネットワーク接続の状態。 可能な値は、`unknown`、`attempted`、`succeeded`、`blocked`、`failed` です。|
|urlParameters|文字列|リンク先URLのパラメーター(サフィックス)。|

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