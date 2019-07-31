---
title: educationSubmissionIndividualRecipient リソースの種類
description: 'EducationSubmissionRecipient のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2eecdc7e7ddd30ecad9a520b42cd11df9565fa71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972510"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a>educationSubmissionIndividualRecipient リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[EducationSubmissionRecipient](educationsubmissionrecipient.md)のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。  


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
  "suppressions": []
}
-->
