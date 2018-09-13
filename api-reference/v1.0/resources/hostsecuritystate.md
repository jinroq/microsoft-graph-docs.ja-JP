# <a name="hostsecuritystate-resource-type"></a>hostSecurityState リソースの種類

ホストに関するステートフルな情報 (デバイス、コンピューターなど) が含まれます。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|FQDN|文字列|ホスト FQDN (完全修飾ドメイン名) (たとえば、 `machine.company.com`)。|
|isAzureAadJoined|ブール値|ホストが Azure Active Directory ドメイン サービスに参加しているドメインである場合は true。|
|isAzureAadRegistered|ブール値|Azure Active Directory Device Registration (BYOD デバイスは、起業によって完全に管理されていません) で登録されたホストの場合は true。|
|isHybridAzureDomainJoined|ブール値|ホストが、オンプレミスの Active Directory ドメインに参加しているドメインである場合は true。|
|netBiosName|文字列|DNS ドメイン名を持たないローカル ホスト名|
|os|文字列|文字列 (たとえば、Windows10、MacOS、RHEL など)。|
|privateIpAddress|文字列|警告時の (ルーティングできない) プライベート IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918) 参照)。|
|publicIpAddress|文字列|警告時の公的にルーティング可能な IPv4 アドレスまたは IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918) 参照)。|
|riskScore|文字列|プロバイダーが生成 / 計算したホストのリスク スコアです。  1 パーセンテージ相当する 0 - 1 の値の範囲を推奨します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
