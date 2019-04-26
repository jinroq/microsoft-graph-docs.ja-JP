---
title: プラン、listitem リソースの種類
description: '**plan**は、タスクのチェックリストの項目を表します。 タスクのチェックリストは、checklistItems オブジェクトによって表されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: deb168fa123c893d0d3793b0e67f65b6da2819b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344502"
---
# <a name="plannerchecklistitem-resource-type"></a>プラン、listitem リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plan**は、タスクのチェックリストの項目を表します。 タスクのチェックリストは、 [checklistItems オブジェクト](plannerchecklistitems.md)によって表されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ischecked|Boolean|値は`true` 、アイテムがチェックされ`false`ているかどうかを示します。|
|lastModifiedBy|[identitySet](identityset.md)| 読み取り専用です。 これを最後に変更するユーザー ID。|
|lastModifiedDateTime|DateTimeOffset|読み取り専用。 この時刻が最後に変更された日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|orderHint|String|チェックリストの項目の相対的な順序を設定するために使用します。 この形式は、[ここで](planner-order-hint-format.md)説明するように定義されています。|
|title|String|チェックリストアイテムのタイトル|

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
