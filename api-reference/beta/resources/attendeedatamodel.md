---
title: attendeeDataModel リソースの種類
description: 出席者の種類です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8659b88cae8b9d2a94177593da40b61363fa23b
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057405"
---
# <a name="attendeedatamodel-resource-type"></a>attendeeDataModel リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議に含まれている個人またはリソースを表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "type"
  ],
  "@odata.type": "microsoft.graph.attendeeDataModel"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|type|attendeeType| 出席者の種類です。 使用可能な値は`required`、 `optional`、 `resource`、です。 現時点では、参加者が人物の場合、 [findの会議時間](../api/user-findmeetingtimes.md)は常にその`required`人物の種類を考慮します。|
|emailAddress|[emailAddress](emailaddress.md)|参加者の名前と SMTP アドレスが含まれます。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeedatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->