---
title: educationLinkResource リソースの種類
description: educationResource のサブクラス。 このリソースはリンクであり、それに関連付けられている追加のデータはありません。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 09e7c7c5070d6f8f288dbf18d6fb9ce81b456092
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542881"
---
# <a name="educationlinkresource-resource-type"></a>educationLinkResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)のサブクラス。 このリソースはリンクであり、それに関連付けられている追加のデータはありません。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|link|String|リソースへの URL。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationlinkresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
