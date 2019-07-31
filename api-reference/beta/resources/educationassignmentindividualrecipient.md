---
title: educationAssignmentIndividualRecipient リソースの種類
description: 'プロパティへの割り当ての中で使用されます。 個別の受信者一覧に設定すると、クラス内の学生が選択されます。 '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7408382cadcb53d857bb36b06702f7857d64a8f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006452"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>educationAssignmentIndividualRecipient リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロパティへの[割り当て](educationassignment.md)の中で使用されます。 個別の受信者一覧に設定した場合、クラス内の学生は、割り当てが発行されたときに送信オブジェクトを受け取ります。

このリソースは[educationAssignmentRecipient](educationassignmentrecipient.md)のサブクラスです。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|recipients|文字列コレクション|受信者の id のコレクション。|

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
  "suppressions": []
}
-->
