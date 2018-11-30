---
title: domainDnsUnavailableRecord リソースの種類
description: ドメイン エンティティのナビゲーション プロパティの**serviceConfigurationRecords**のクエリを実行すると、1 つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、および DomainDnsTxtRecord のエンティティが表示されます。 これらのエンティティは、Microsoft Online Services で使用するドメインに、ドメインのゾーン ファイルに追加する必要がありますどのような DNS レコードを指定します。 このようなエンティティを生成できない場合は、DomainDnsUnavailableRecord のエンティティが返されます。 DomainDnsRecord エンティティから継承されます。
ms.openlocfilehash: 3eee5a814e7629ae603dc41670429fa82b85495f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024120"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>domainDnsUnavailableRecord リソースの種類

[Domain](domain.md) エンティティのナビゲーション プロパティ **serviceConfigurationRecords** に対してクエリを実行すると、[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsTxtRecord](domaindnstxtrecord.md) エンティティのいずれか 1 つ以上が返される場合があります。これらのエンティティは、ドメインを Microsoft オンライン サービスで使用する前に、そのドメインのゾーン ファイルに追加する必要のある DNS レコードを示します。このようなエンティティを生成できない場合、代わりに DomainDnsUnavailableRecord エンティティが返されます。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|説明|String|**DomainDnsUnavailableRecord** エンティティが返される理由を示します。 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->