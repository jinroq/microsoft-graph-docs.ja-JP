---
title: educationOrganization リソースの種類
description: '教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 49afe12f4897df80ce78ba28a024883cefeb0a96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340482"
---
# <a name="educationorganization-resource-type"></a>educationOrganization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。  

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|String| 組織の説明。|
|displayName|String| 組織の表示名。|
|externalSource|string| この組織の作成元のソース。 可能な値は、`sis`、`manual`、`unknownFutureValue` です。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
