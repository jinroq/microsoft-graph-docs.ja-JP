# <a name="domaindnsrecord-resource-type"></a>domainDnsRecord リソースの種類

テナント内の各ドメインでは、Microsoft オンライン サービスでドメインを使用できるようにするために、DNS レコードをそのドメインの DNS ゾーン ファイルに追加しなければならない場合があります。**DomainDnsRecord** エンティティはこのような DNS レコードの表示に使用されます。[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) エンティティのベース エンティティ。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|ID|文字列| このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。|
|isOptional|ブール値| False の場合、このレコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。 |
|ラベル|文字列| DNS ホストで DNS レコードの名前を設定するときに使用する値。 |
|recordType|文字列| このエンティティが表す DNS レコードの種類を示します。</br></br>値は次のいずれかを指定できます。*CName*、*Mx*、*Srv*、*Txt*</br></br>キー |
|supportedService|文字列| Microsoft オンライン サービスまたはこの DNS レコードに依存している機能。</br></br>次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*|
|ttl|Int32| DNS ホストの DNS レコードの Time to Live (TTL) のプロパティを構成するときに使用する値です。null 許容ではありません |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->