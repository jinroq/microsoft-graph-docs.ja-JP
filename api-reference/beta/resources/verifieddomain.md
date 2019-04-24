---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。 組織エンティティの**verifiedDomains**プロパティは、 **VerifiedDomain**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: c13c3b3da39b762c26d637deaddafbee5da40160
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454038"
---
# <a name="verifieddomain-resource-type"></a>verifiedDomain リソースの種類

テナントのドメインを指定します。 [組織](organization.md)エンティティの**verifiedDomains**プロパティは、 **VerifiedDomain**のコレクションです。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|capabilities|String|「電子メール」、「OfficeCommunicationsOnline」など。|
|isDefault|ブール型 (Boolean)|                これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。            |
|isinitial|ブール値|これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。|
|name|String|ドメイン名。「contoso.onmicrosoft.com」など。|
|type|String|「管理対象」など。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
