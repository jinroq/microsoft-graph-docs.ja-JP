---
title: domainDnsUnavailableRecord リソースの種類
description: ドメインエンティティのナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、または domaindnst record エンティティが返される場合があります。 これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。 そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。 domaindnsrecord エンティティから継承されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe3c1eeae7ae3ddb634a3c120332dd8d8996f41c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535033"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>domainDnsUnavailableRecord リソースの種類

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
