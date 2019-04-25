---
title: attendeeAvailability リソースの種類
description: 出席者の空き時間。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 396c53b8d03f573c214dcf43a3637cf06f412a33
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535607"
---
# <a name="attendeeavailability-resource-type"></a>attendeeAvailability リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

出席者の空き時間。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|attendee|[attendeeBase](attendeebase.md)|出席者の電子メールアドレスと種類。個人またはリソースのいずれかを指定します。また、必要かどうかは、ユーザーの場合はオプションです。|
|availability|freeBusyStatus| 出席者の空き時間の状態。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->