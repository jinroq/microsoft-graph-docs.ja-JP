---
title: domainDnsMxRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された MX レコードを表します。 DomainDnsRecord エンティティから継承されます。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d837ce660ebceda300d63d428b92836b3173fba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032663"
---
# <a name="domaindnsmxrecord-resource-type"></a>domainDnsMxRecord リソースの種類

テナント内の特定のドメインの DNS ゾーンファイルに追加された MX レコードを表します。 [Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。 ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| このエンティティに割り当てられている一意の識別子。 Null 許容ではありません。読み取り専用です。|
|isOptional|Boolean| False の場合、MX レコードは、Microsoft Online Services がドメインで正しく動作するように、DNS ホストで顧客によって構成されている必要があります。 |
|label|String| DNS ホストで MX レコードの*alias/host/name*プロパティを構成する場合に使用される値です。 |
|mailExchange|String| DNS ホストで MX レコードの*応答/宛先/値*を構成する場合に使用される値です。|
|優先順位|Int32| DNS ホストで MX レコードの*Preference/Priority*プロパティを構成する場合に使用される値です。 |
|recordType|String| DNS レコードの種類。 値は常に*Mx*です。 Key |
|supportedService|String| この MX レコードに依存している Microsoft Online サービスまたは機能。</br></br>**Null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 **、 *Orgidauthentication*、 *Yammer*、 *Intune* |
|ttl|Int32| DNS ホストで MX レコードの*time to live (ttl)* プロパティを構成する場合に使用する値です。 Null 許容ではない |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
