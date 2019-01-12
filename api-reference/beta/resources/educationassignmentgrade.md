---
title: educationAssignmentGrade リソースの種類
description: " ただし、このサブクラスは、すべてのタイプ (点、合格/不合格、) のグレーディングの"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: ecdd92c84399ee17d2808301d997830725fb5642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982359"
---
# <a name="educationassignmentgrade-resource-type"></a>educationAssignmentGrade リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

提出書類の**成績**のオブジェクトを表します。 これは、抽象型はインスタンス化します。ただし、グレーディング、(ポイント、合格/不合格、) のすべての種類は、このリソースの種類のサブクラスです。 このオブジェクトは、グレーディングを行っているにも追跡します。 **Submission.grade**プロパティで使用されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| グレーディングをしたユーザーです。 |
|gradedDateTime|DateTimeOffset| グレードがこの送信オブジェクトに適用されたときの時点です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
