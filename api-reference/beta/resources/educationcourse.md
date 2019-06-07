---
title: educationCourse リソースの種類
description: クラスのコース情報を表します。
author: mlafleur
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eac609f787621e30d4707d477296fc53af77dad0
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764769"
---
# <a name="educationcourse-resource-type"></a>educationCourse リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

クラスのコース情報を表します。 [educationClass](educationclass.md) 内で使用します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型   | 説明                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | String | コースの一意識別子。         |
| description  | String | コースの説明。                |
| displayName  | 文字列 | コースの名前を指定します。                       |
| externalId   | String | 同期システムからのコースの ID。 |
| subject      | String | コースの件名。                    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCourse"
}-->

```json
{
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationCourse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
