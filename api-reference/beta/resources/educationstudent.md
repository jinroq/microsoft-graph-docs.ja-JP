---
title: educationStudent リソースの種類
description: ユーザーの primaryRole が `student` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: f87bbe9b15f89660a166c0ca1d9a1aaa4bbd9eff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878121"
---
# <a name="educationstudent-resource-type"></a>educationStudent リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|birthDate|Date| 学生の生年月日。|
|externalId|String| ソース システムの学生の ID。|
|gender|`educationGender enumeration`| 使用可能な値: `female`、`male`、`other`、`unkownFutureValue`。|
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
