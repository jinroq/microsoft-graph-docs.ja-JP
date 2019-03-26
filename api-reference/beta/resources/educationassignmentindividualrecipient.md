---
title: educationAssignmentIndividualRecipient リソースの種類
description: 'プロパティへの割り当ての中で使用されます。 個別の受信者一覧に設定すると、クラス内の学生が選択されます。 '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 736345901faeeb4d3fab4d417752b684f1e19307
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799992"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>educationAssignmentIndividualRecipient リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロパティへの[割り当て](educationassignment.md)の中で使用されます。 個別の受信者一覧に設定した場合、クラス内の学生は、割り当てが発行されたときに送信オブジェクトを受け取ります。

このリソースは[educationAssignmentRecipient](educationassignmentrecipient.md)のサブクラスです。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|recipients|String collection|受信者の id のコレクション。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
