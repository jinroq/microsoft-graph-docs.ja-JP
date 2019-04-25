---
title: domaindnsrecord リソースの種類
description: テナント内のドメインごとに、ドメインを Microsoft Online Services で使用できるようにするには、ドメインの dns ゾーンファイルに dns レコードを追加することが必要になることがあります。 **domaindnsrecord**エンティティは、そのような DNS レコードを提示するために使用されます。 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、および DomainDnsSrvRecord エンティティの基本エンティティ。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b7b04e65da67bc61e3f3b91ed3dae7cba70a3d27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543155"
---
# <a name="domaindnsrecord-resource-type"></a>domaindnsrecord リソースの種類

テナント内のドメインごとに、ドメインを Microsoft Online Services で使用できるようにするには、ドメインの dns ゾーンファイルに dns レコードを追加することが必要になることがあります。 **domaindnsrecord**エンティティは、そのような DNS レコードを提示するために使用されます。 [DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md) 、および[DomainDnsSrvRecord](domaindnssrvrecord.md)エンティティの基本エンティティ。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。 ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| このエンティティに割り当てられている一意の識別子。 null 許容ではありません。読み取り専用です。|
|isoptional|ブール値| false の場合、このレコードは、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって構成されている必要があります。 |
|label|String| dns ホストで dns レコードの名前を構成するときに使用される値です。 |
|recordType|String| このエンティティが表す DNS レコードの種類を示します。</br></br>この値には、 *CName*、 *Mx*、 *Srv*、 *Txt*のいずれかを指定できます。</br></br>キー |
|supportedservice|String| この DNS レコードに依存している Microsoft Online サービスまたは機能。</br></br>**null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 **、 *orgidauthentication*、 *Yammer*、 *Intune*|
|ttl|Int32| dns ホストで dns レコードの time-to-live (ttl) プロパティを構成する場合に使用する値です。 null 許容ではない |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
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
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
