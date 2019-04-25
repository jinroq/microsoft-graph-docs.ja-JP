---
title: educationAssignmentGrade リソースの種類
description: " ただし、すべての種類の種類 (ポイント、合格/失敗など) は、この"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5ca13ba057ef000a468d910d49288d9ae8e0c962
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543022"
---
# <a name="educationassignmentgrade-resource-type"></a>educationAssignmentGrade リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提出物の**学年**オブジェクトを表します。 これは、インスタンス化されない抽象型です。ただし、すべての種類の種類 (ポイント、合格/失敗など) は、このリソースの種類のサブクラスです。 また、このオブジェクトは、対象とするユーザーを追跡します。 これは、"**成績**" プロパティで使用されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| 対象をしたユーザー。 |
|gradedDateTime|DateTimeOffset| 成績がこの提出物オブジェクトに適用された時点での時間。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
