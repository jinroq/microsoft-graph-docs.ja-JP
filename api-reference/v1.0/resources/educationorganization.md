---
title: educationOrganization リソースの種類
description: 教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c62e65ffb6c6a0e3a8af92bda6a8b1e1c241ada7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032635"
---
# <a name="educationorganization-resource-type"></a>educationOrganization リソースの種類

教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|String| 組織の説明。|
|displayName|String| 組織の表示名。|
|externalSource|educationExternalSource| この組織の作成元のソース。 使用可能な値: `sis`、`manual`、`unknownFutureValue`。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
