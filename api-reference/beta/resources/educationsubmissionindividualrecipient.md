---
title: educationSubmissionIndividualRecipient リソースの種類
description: 'educationSubmissionRecipient のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: de58dc743cd50f0e31021b4651bb0a3b3b192197
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340556"
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
  "suppressions": []
}
-->
