---
title: educationOrganization リソースの種類
description: '教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 122717952781cd8effe415fb01b07ec9bf71143d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507181"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationorganization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
