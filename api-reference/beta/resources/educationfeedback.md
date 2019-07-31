---
title: educationFeedback リソースの種類
description: 教師から学生へのフィードバック。 このプロパティは、フィードバックのテキスト部分と who の両方を表します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7300c5f2d46a3a60a104288d8ee9559e6cf5fd2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006417"
---
# <a name="educationfeedback-resource-type"></a>educationFeedback リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

教師から学生へのフィードバック。 このプロパティは、フィードバックのテキスト部分と who の両方を表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|フィードバック|[identitySet](identityset.md)|フィードバックを作成したユーザー。|
|フィードバック Datetime|DateTimeOffset|フィードバックが提供された時点の時間。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|text|[itemBody](itembody.md)|フィードバック.|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String (timestamp)",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
