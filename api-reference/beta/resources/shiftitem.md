---
title: "\"佐々木 ftitem\" リソースの種類"
description: "\"佐々木 ftitem\" は、シフトのバージョンを表します。"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd5b3d224e60fc3f21b4d484952c7a2643b02407
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343039"
---
# <a name="shiftitem-resource-type"></a>"佐々木 ftitem" リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[シフト](shift.md)のバージョンを表します。

## <a name="properties"></a>プロパティ
| プロパティ                         | 型                    | 説明                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | string                  | のメモ`shiftItem`。      |
| displayName               | string                  | の名前`shiftItem`。 |
| startDateTime               | DateTimeOffset                  | の開始日時`shiftItem`。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 必須です。 |
| endDateTime               | DateTimeOffset                 | の終了日時`shiftItem`。 必須です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| theme | scheduleentitytheme   |  サポートされている色: 白。水色緑青紫色ピンクイエロー灰色darkBlue;darkGreen;darkPurple;darkPink;darkYellow。 |
| アクティビティ    | [shiftActivity](shiftactivity.md)コレクション   | 従業員がいつ、どのような時間帯に勤務しているかを詳細に説明できる、シフトの増分部分。 たとえば、割り当て、またはスケジュールされた休憩またはランチ。 必須。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
