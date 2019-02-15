---
title: locationConstraintItem リソースの種類
description: 会議の場所に関して、クライアントが表明している条件です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8e0b14096d8be66a6aab6d4e73cf0941d7db7b5c
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057002"
---
# <a name="locationconstraintitem-resource-type"></a>locationConstraintItem リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議の場所に関して、クライアントが表明している条件です。

[locationDataModel](locationdatamodel.md)から派生します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
| address | [physicalAddress](physicaladdress.md) |場所の番地。 |
| coordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 場所の地理的座標と標高。 |
| displayName  | 文字列 | 場所に関連付けられた名前。                       |
| locationEmailAddress | String | 場所のメール アドレス (省略可能)。 |
| locationUri | String | 場所を表す URI (省略可能)。 |
| resolveAvailability | Boolean | true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user-findmeetingtimes.md) は空いている別のリソースを検索します。false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。既定値は true です。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraintitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
