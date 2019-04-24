---
title: educationStudent リソースの種類
description: ユーザーの primaryRole が `student` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 683a290806f9a70f97bda4aa9429a64578fbcd97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463559"
---
# <a name="educationstudent-resource-type"></a>educationStudent リソースの種類

ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|birthDate|Date| 学生の生年月日。|
|externalId|String| ソース システムの学生の ID。|
|gender|educationGender| 使用可能な値は`female`、 `male`、 `other`、 `unknownFutureValue`、です。|
|grade|String|学生の現在の学年。|
|graduationYear|String| 学生が学校から卒業する年。|
|studentNumber|String| 学生番号。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
