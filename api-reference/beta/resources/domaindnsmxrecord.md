---
title: domainDnsMxRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された MX レコードを表します。 domaindnsrecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 09af66a522d99645540ec24324c82f565eaedb1e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535124"
---
# <a name="domaindnsmxrecord-resource-type"></a>domainDnsMxRecord リソースの種類

テナント内の特定のドメインの DNS ゾーンファイルに追加された MX レコードを表します。 [domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。 ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| このエンティティに割り当てられている一意の識別子。 null 許容ではありません。読み取り専用です。|
|isoptional|ブール値| false の場合、MX レコードは、Microsoft Online Services がドメインで正しく動作するように、DNS ホストで顧客によって構成されている必要があります。 |
|label|String| DNS ホストで MX レコードの*alias/host/name*プロパティを構成する場合に使用される値です。 |
|mailexchange|String| DNS ホストで MX レコードの*応答/宛先/値*を構成する場合に使用される値です。|
|優先順位|Int32| DNS ホストで MX レコードの*Preference/Priority*プロパティを構成する場合に使用される値です。 |
|recordType|String| DNS レコードの種類。 値は常に*Mx*です。 キー |
|supportedservice|String| この MX レコードに依存している Microsoft Online サービスまたは機能。</br></br>**null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 **、 *orgidauthentication*、 *Yammer*、 *Intune* |
|ttl|Int32| DNS ホストで MX レコードの*time to live (ttl)* プロパティを構成する場合に使用する値です。 null 許容ではない |

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
