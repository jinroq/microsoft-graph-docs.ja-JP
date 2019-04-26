---
title: domaindnst・ record リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された TXT レコードを表します。 domaindnsrecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14280f7ddaa172960a269a22255db4ea3e44dc61
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334509"
---
# <a name="domaindnstxtrecord-resource-type"></a>domaindnst・ record リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナント内の特定のドメインの DNS ゾーンファイルに追加された TXT レコードを表します。 [domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。 ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| このエンティティに割り当てられている一意の識別子。 null 許容ではありません。読み取り専用です。 |
|isoptional|Boolean| false の場合は、Microsoft Online Services がドメインで正しく動作するように、DNS ホストで顧客によって TXT レコードが構成されている必要があります。 |
|label|String| DNS ホストで TXT レコードの*name*プロパティを構成する場合に使用する値です。|
|recordType|String| DNS レコードの種類。 値は常に*Txt*です。 Key |
|supportedservice|String| Microsoft Online サービスまたはこの TXT レコードに依存している機能。</br></br>**null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 **、 *orgidauthentication*、 *Yammer*、 *Intune* |
|text|String| DNS ホストで*text*プロパティを構成する場合に使用される値です。 |
|ttl|Int32| DNS ホストで MX レコードの*time to live (ttl)* プロパティを構成する場合に使用する値です。 null 許容ではない |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "canonicalName": "String",
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
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
