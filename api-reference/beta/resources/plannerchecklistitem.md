---
title: plannerChecklistItem リソースの種類
description: '**PlannerChecklistItem**リソースは、タスクのチェックリストの項目を表します。 タスクのチェックリストは、checklistItems オブジェクトによって表されます。'
ms.openlocfilehash: 846c1877fb421c9070eff7c041983367a7beb29b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069762"
---
# <a name="plannerchecklistitem-resource-type"></a>plannerChecklistItem リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**PlannerChecklistItem**リソースはタスクのチェックリスト内の項目を表します。タスクのチェックリストは、[checklistItems オブジェクト](plannerchecklistitems.md)で表されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|isChecked|Boolean|項目がチェックされた場合は `true`、それ以外の場合は `false` です。|
|lastModifiedBy|[identitySet](identityset.md)| 読み取り専用です。これを最後に変更したユーザーの ID。|
|lastModifiedDateTime|DateTimeOffset|読み取り専用です。これを最後に変更した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|orderHint|String|チェックリストでの項目の相対順序を設定するのに使用します。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|
|タイトル|String|チェックリスト項目のタイトル|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->