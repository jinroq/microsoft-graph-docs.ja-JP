---
title: domainDnsCnameRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された CNAME レコードを表します。DomainDnsRecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 226f067756517771b1d86f053d48268b905dd930
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990496"
---
# <a name="domaindnscnamerecord-resource-type"></a>domainDnsCnameRecord リソースの種類

テナント内の特定のドメインの DNS ゾーン ファイルに追加された CNAME レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。


## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|canonicalName|String| CNAME レコードの正規名。DNS ホストで CNAME レコードを構成するために使用されます。 |
|id|String| このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用。|
|isOptional|Boolean| false の場合、ドメインが指定された Microsoft Online Services が適切に機能するには、CNAME レコードが DNS ホストで顧客によって構成されている必要があります。null 許容ではありません |
|label|String| DNS ホストで CNAME レコードの*エイリアス/ホスト/名前*を構成する場合に使用される値です。 |
|recordType|String| DNS レコードの種類。この値は常に *CName* です。キー|
|supportedService|String| Microsoft オンライン サービスまたはこの CNAME レコードに依存している機能。</br></br>次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*|
|ttl|Int32| DNS ホストで CNAME レコードの Time To Live (TTL) のプロパティを構成するときに使用する値。null 許容ではありません |

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
