---
title: domainDnsUnavailableRecord リソースの種類
description: ドメイン エンティティのナビゲーション プロパティの**serviceConfigurationRecords**のクエリを実行すると、1 つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、および DomainDnsTxtRecord のエンティティが表示されます。 これらのエンティティは、Microsoft Online Services で使用するドメインに、ドメインのゾーン ファイルに追加する必要がありますどのような DNS レコードを指定します。 このようなエンティティを生成できない場合は、DomainDnsUnavailableRecord のエンティティが返されます。 DomainDnsRecord エンティティから継承されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99da0448d75375b84bb37c05102c1f702c222a25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982793"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>domainDnsUnavailableRecord リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[Domain](domain.md) エンティティのナビゲーション プロパティ **serviceConfigurationRecords** に対してクエリを実行すると、[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsTxtRecord](domaindnstxtrecord.md) エンティティのいずれか 1 つ以上が返される場合があります。これらのエンティティは、ドメインを Microsoft オンライン サービスで使用する前に、そのドメインのゾーン ファイルに追加する必要のある DNS レコードを示します。このようなエンティティを生成できない場合、代わりに DomainDnsUnavailableRecord エンティティが返されます。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|説明|String|**DomainDnsUnavailableRecord** エンティティが返される理由を示します。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
