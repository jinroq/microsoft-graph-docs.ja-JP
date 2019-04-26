---
title: domainDnsSrvRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加される SRV レコードを表します。 domaindnsrecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28c590ff210952fc5d54ace61c08348383ce393a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562793"
---
# <a name="domaindnssrvrecord-resource-type"></a>domainDnsSrvRecord リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナント内の特定のドメインの DNS ゾーンファイルに追加される SRV レコードを表します。 [domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。 ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| このエンティティに割り当てられている一意の識別子。 null 許容ではありません。読み取り専用です。|
|isoptional|Boolean| false の場合、SRV レコードは、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって構成されている必要があります。 |
|label|String| DNS ホストで SRV レコードの*name*プロパティを構成する場合に使用される値です。 |
|nametarget|String| DNS ホストで SRV レコードの*Target*プロパティを構成する場合に使用する値です。 |
|ポート|Int32| DNS ホストで SRV レコードの*port*プロパティを構成する場合に使用する値です。 |
|priority|Int32| DNS ホストで SRV レコードの*priority*プロパティを構成する場合に使用する値です。 |
|プロトコール|String| DNS ホストで SRV レコードの*protocol*プロパティを構成する場合に使用する値です。 |
|recordType|String|  DNS レコードの種類。 値は常に*Srv*です。 キー |
|service|String| DNS ホストで SRV レコードの*service*プロパティを構成する場合に使用する値です。 |
|supportedservice|String| この SRV レコードに依存している Microsoft Online サービスまたは機能。</br></br>**null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 **、 *orgidauthentication*、 *Yammer*、 *Intune* |
|ttl|Int32| DNS ホストで SRV レコードの*タイムツーリブ (ttl)* プロパティを構成する場合に使用する値です。 null 許容ではない |
|weight|Int32| DNS ホストで SRV レコードの*weight*プロパティを構成する場合に使用する値です。 |

## <a name="relationships"></a>関係
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
