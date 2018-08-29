# <a name="domaindnssrvrecord-resource-type"></a>domainDnsSrvRecord リソースの種類

テナント内の特定のドメインの DNS ゾーン ファイルに追加された SRV レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|ID|文字列| このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。|
|isOptional|ブール値| False の場合、SRV レコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。 |
|ラベル|文字列| DNS ホストで SRV レコードの *name* プロパティを構成する場合に使用される値です。 |
|nameTarget|文字列| DNS ホストで SRV レコードの *Target* プロパティを構成する場合に使用する値です。 |
|ポート|Int32| DNS ホストで SRV レコードの *port* プロパティを構成する場合に使用する値です。 |
|優先度|Int32| DNS ホストで SRV レコードの *priority* プロパティを構成する場合に使用する値です。 |
|プロトコル|文字列| DNS ホストで SRV レコードの *protocol* プロパティを構成する場合に使用する値です。 |
|recordType|文字列|  DNS レコードの種類。この値は常に *Srv* です。キー |
|サービス|文字列| DNS ホストで SRV レコードの *service* プロパティを構成する場合に使用する値です。 |
|supportedService|文字列| Microsoft オンライン サービスまたはこの SRV レコードに依存している機能。</br></br>次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune* |
|ttl|Int32| DNS ホストで SRV レコードの *Time to Live (TTL)* のプロパティを構成するときに使用する値です。null 許容ではありません |
|ウェイト|Int32| DNS ホストで SRV レコードの *weight* プロパティを構成する場合に使用する値です。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->