---
title: genericerror リソースの種類
description: 汎用エラー。
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547499"
---
# <a name="genericerror-resource-type"></a>genericerror リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

汎用エラー。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
| メッセージ​​ | String | エラー メッセージ。 |
| code | String | エラーコード。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/genericerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
