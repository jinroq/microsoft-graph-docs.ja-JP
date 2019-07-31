---
title: governanceSubject リソースの種類
description: 特権 Id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 26f6c6904de97fc96eb1b29b9bcbc376bcf69c61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005976"
---
# <a name="governancesubject-resource-type"></a>governanceSubject リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権 Id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。


## <a name="properties"></a>プロパティ
| プロパティ  | 型       |説明|
|:----------|:----------|:----------|
|id         |文字列     | 件名の id。|
|type       |String     |件名の種類。 この値は、 ``User``、 ``Group``、と``ServicePrincipal``することができます。|
|displayName|文字列型 (String)     |件名の表示名。|
|メール      |String     |ユーザーの件名の電子メールアドレス。 件名が他の種類の場合は、空になります。|
|principalName|String   |ユーザーの件名のプリンシパル名。 件名が他の種類の場合は、空になります。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
