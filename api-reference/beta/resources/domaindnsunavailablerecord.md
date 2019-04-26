---
title: domainDnsUnavailableRecord リソースの種類
description: ドメインエンティティのナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、または domaindnst record エンティティが返される場合があります。 これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。 そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。 domaindnsrecord エンティティから継承されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f641170673a1b42f8a15c268ac08bf8097a7dfcb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340673"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>domainDnsUnavailableRecord リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ドメイン](domain.md)エンティティに対してナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)、または[が返されることがあります。domaindnst・ record](domaindnstxtrecord.md)エンティティ。 これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。 そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。 [domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。

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
