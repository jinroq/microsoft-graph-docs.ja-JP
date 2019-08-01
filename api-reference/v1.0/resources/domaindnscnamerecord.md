---
title: domainDnsCnameRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された CNAME レコードを表します。 DomainDnsRecord エンティティから継承されます。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 397886a000b18dfb4a946d29f7459cc79e0d27a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029443"
---
# <a name="domaindnscnamerecord-resource-type"></a>domainDnsCnameRecord リソースの種類

テナント内の特定のドメインの DNS ゾーンファイルに追加された CNAME レコードを表します。 [Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。


## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。 ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|canonicalName|String| CNAME レコードの標準名。 DNS ホストで CNAME レコードを構成するために使用します。 |
|id|String| このエンティティに割り当てられている一意の識別子。 Null 非許容、読み取り専用|
|isOptional|Boolean| False の場合は、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって CNAME レコードが構成されている必要があります。 Null 許容ではない |
|label|String| DNS ホストで CNAME レコードの*エイリアス/ホスト/名前*を構成する場合に使用される値です。 |
|recordType|String| DNS レコードの種類。 値は常に*CName*です。 Key|
|supportedService|String| この CNAME レコードに依存している Microsoft Online サービスまたは機能。</br></br>**Null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 **、 *Orgidauthentication*、 *Yammer*、 *Intune*|
|ttl|Int32| DNS ホストで CNAME レコードの time to live (ttl) プロパティを構成する場合に使用する値です。 Null 許容ではない |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
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
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
