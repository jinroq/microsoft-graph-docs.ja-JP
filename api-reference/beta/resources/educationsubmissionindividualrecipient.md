---
title: educationSubmissionIndividualRecipient リソースの種類
description: 'educationSubmissionRecipient のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8660ec569362d8170d15de86073c0ef59c9ec0a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507061"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a>educationSubmissionIndividualRecipient リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationSubmissionRecipient](educationsubmissionrecipient.md)のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。  


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|userId|String|提出物が割り当てられているユーザーのユーザー ID。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
