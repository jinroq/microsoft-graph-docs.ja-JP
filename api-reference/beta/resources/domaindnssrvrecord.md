---
title: domainDnsSrvRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加される SRV レコードを表します。 DomainDnsRecord エンティティから継承されます。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b4d96bf39581b0d49c969239bbffc4a9cf97d067
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973112"
---
# <a name="domaindnssrvrecord-resource-type"></a>domainDnsSrvRecord リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナント内の特定のドメインの DNS ゾーンファイルに追加される SRV レコードを表します。 [Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。 ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| このエンティティに割り当てられている一意の識別子。 Null 許容ではありません。読み取り専用です。|
|isOptional|Boolean| False の場合、SRV レコードは、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって構成されている必要があります。 |
|label|String| DNS ホストで SRV レコードの*name*プロパティを構成する場合に使用される値です。 |
|nameTarget|String| DNS ホストで SRV レコードの*Target*プロパティを構成する場合に使用する値です。 |
|ポート|Int32| DNS ホストで SRV レコードの*port*プロパティを構成する場合に使用する値です。 |
|priority|Int32| DNS ホストで SRV レコードの*priority*プロパティを構成する場合に使用する値です。 |
|プロトコール|String| DNS ホストで SRV レコードの*protocol*プロパティを構成する場合に使用する値です。 |
|recordType|String|  DNS レコードの種類。 値は常に*Srv*です。 Key |
|service|String| DNS ホストで SRV レコードの*service*プロパティを構成する場合に使用する値です。 |
|supportedService|String| この SRV レコードに依存している Microsoft Online サービスまたは機能。</br></br>**Null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 **、 *Orgidauthentication*、 *Yammer*、 *Intune* |
|ttl|Int32| DNS ホストで SRV レコードの*タイムツーリブ (ttl)* プロパティを構成する場合に使用する値です。 Null 許容ではない |
|weight|Int32| DNS ホストで SRV レコードの*weight*プロパティを構成する場合に使用する値です。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
