---
title: 診断リソースの種類
description: OneNote の操作に関するエラーまたは警告に関する情報。
localization_priority: Normal
ms.openlocfilehash: ef495374f84e0df887198b38a5c8488987a59343
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535215"
---
# <a name="diagnostic-resource-type"></a>診断リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneNote の操作に関するエラーまたは警告に関する情報。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|メッセージ​​|String|エラーまたは警告を発生させた条件を説明するメッセージ。|
|url|String|この問題に関するドキュメントへのリンク。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/diagnostic.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
