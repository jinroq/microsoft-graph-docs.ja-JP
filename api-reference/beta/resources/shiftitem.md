---
title: "\"佐々木 ftitem\" リソースの種類"
description: "\"佐々木 ftitem\" は、シフトのバージョンを表します。"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ff829ca0f43124404b4b99b048c9919368b6009
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657708"
---
# <a name="shiftitem-resource-type"></a>"佐々木 ftitem" リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[シフト](shift.md)のバージョンを表します。

## <a name="properties"></a>プロパティ
| プロパティ                         | 型                    | 説明                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | `string`                  | のメモ`shiftItem`。      |
| displayName               | `string`                  | の名前`shiftItem`。 |
| startDateTime               | `DateTimeOffset`                  | の開始日時`shiftItem`。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。 必須。 |
| endDateTime               | `DateTimeOffset`                  | の終了日時`shiftItem`。 必須。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。 |
| theme | `enum`   |    |  |  | サポートされている色: 白。水色緑青紫色ピンクイエロー灰色darkBlue;darkGreen;darkPurple;darkPink;darkYellow。 |
| アクティビティ    | `collection([shiftActivity](shiftactivity.md))`    | 従業員がいつ、どのような時間帯に勤務しているかを詳細に説明できる、シフトの増分部分。 たとえば、割り当て、またはスケジュールされた休憩またはランチ。 必須。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "Day shift",
  "notes": "Please do inventory as part of your shift.",
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-12T00:00:00Z",
  "theme": "blue",
  "activities": [
    {
      "isPaid": true,
      "startDateTime": "2019-03-11T15:00:00Z",
      "endDateTime": "2019-03-11T15:15:00Z",
      "code": "",
      "displayName": "Lunch"
    }
  ]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
