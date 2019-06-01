---
title: domainDnsUnavailableRecord リソースの種類
description: ドメインエンティティのナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、または Domaindnst record エンティティが返される場合があります。 これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。 そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。 DomainDnsRecord エンティティから継承されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6f3a392988d0742940e02773965031917f014527
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657099"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>domainDnsUnavailableRecord リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ドメイン](domain.md)エンティティに対してナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)、または[が返されることがあります。Domaindnst・ Record](domaindnstxtrecord.md)エンティティ。 これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。 そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。 [Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。 ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|String|**DomainDnsUnavailableRecord**エンティティが返される理由を示します。 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
