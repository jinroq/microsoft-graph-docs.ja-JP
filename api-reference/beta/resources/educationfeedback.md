---
title: educationFeedback リソースの種類
description: 学生に教師からのフィードバックです。 このプロパティは、両方のテキスト部分に、人とのフィードバックを表します。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0d08f3bc5c7b4882693cdcbba41b364734c6ccef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873564"
---
# <a name="educationfeedback-resource-type"></a>educationFeedback リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

学生に教師からのフィードバックです。 このプロパティは、両方のテキスト部分に、人とのフィードバックを表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|feedbackBy|[identitySet](identityset.md)|フィードバックを作成したユーザー。|
|feedbackDateTime|DateTimeOffset|フィードバックが与えられた瞬間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|text|[itemBody](itembody.md)|フィードバックします。|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
