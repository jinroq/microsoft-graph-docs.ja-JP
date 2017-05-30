# <a name="contract-resource-type"></a>コントラクト リソース型
パートナー テナントがカスタマー テナントとの間で持つ、既存のパートナーシップを表します。

> **重要:**パートナー テナントにのみ存在します。パートナー テナントとは、[Microsoft クラウド ソリューション プロバイダー](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 Syndication、Microsoft Advisor パートナー プログラムのいずれかに含まれている、Microsoft パートナーに所属する Azure AD テナントです。

### <a name="methods"></a>メソッド

| メソッド   | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[コントラクトを取得する](../api/contract_get.md) | コントラクト |特定のコントラクト オブジェクトのプロパティを参照します。 |
|[コントラクトを一覧表示する](../api/contract_list.md) | コントラクト コレクション | パートナー テナントのコントラクトの一覧です。 |

### <a name="properties"></a>プロパティ
| プロパティ   | 型 | 説明 |
|:---------------|:--------|:----------|
|contractType|String|コントラクトの型。<br><br>使用可能な値は次のとおりです。<br> *SyndicationPartner* - この顧客に対し O365 と Intune を排他的に再販し管理するパートナーです。再販し、顧客をサポートします。<br> *BreadthPartner* - この顧客に対し管理上のサポートを提供する能力を備えたパートナーです。ただし、パートナーが顧客に再販売することは許されていません。<br>*ResellerPartner* - シンジケーション パートナーに類似していますが、テナントへの排他的アクセスを持たないパートナーです。シンジケーションの場合、顧客は Microsoft またはその他のパートナーから直接に追加のサブスクリプションを購入することはできません。|
|customerId|Guid|このパートナーシップによって参照されるカスタマー テナントの一意識別子です。カスタマー テナントの組織リソースの ID プロパティに対応します。 |
|defaultDomainName|String|カスタマー テナントの既定のドメイン名のコピーです。顧客とのパートナーシップが確立されるとコピーを作成します。カスタマー テナントの既定のドメイン名が変更された場合は、自動的には更新されません。|
|displayName|String|カスタマー テナントの表示名のコピーです。顧客とのパートナーシップが確立されるとコピーを作成します。カスタマー テナントの表示名が変更された場合は、自動的には更新されません。|
|id|String| パートナーシップの一意識別子です。キー、読み取り専用 |

### <a name="relationships"></a>リレーションシップ
なし


### <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->