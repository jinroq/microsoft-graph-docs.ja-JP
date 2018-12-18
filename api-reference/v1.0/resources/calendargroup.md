---
title: calendarGroup リソースの種類
description: ユーザーの予定表のグループです。
author: angelgolfer-ms
ms.openlocfilehash: 5de023a887622ed0dcc759da7ada6b1e4990b6d5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316906"
---
# <a name="calendargroup-resource-type"></a>calendarGroup リソースの種類

ユーザーの予定表のグループです。

## <a name="methods"></a>メソッド

| メソッド                                                      | 戻り値の型                        | 説明                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [予定表グループを一覧表示する](../api/user-list-calendargroups.md)  | [Calendar](calendar.md) collection | ユーザーの予定表グループを取得します。                               |
| [予定表グループを作成する](../api/user-post-calendargroups.md) | [Calendar](calendar.md)            | 新しい予定表グループを作成します。                                  |
| [予定表グループを取得する](../api/calendargroup-get.md)           | [calendarGroup](calendargroup.md)  | 予定表グループ オブジェクトのプロパティと関係を読み取ります。 |
| [Update](../api/calendargroup-update.md)                    | [calendarGroup](calendargroup.md)  | calendarGroup オブジェクトを更新します。                                  |
| [Delete](../api/calendargroup-delete.md)                    | なし                               | calendarGroup オブジェクトを削除します。                                  |
| [予定表を一覧表示する](../api/calendargroup-list-calendars.md)    | [Calendar](calendar.md) collection | 予定表グループ内の予定表を一覧表示する                           |
| [予定表を作成する](../api/calendargroup-post-calendars.md)   | [Calendar](calendar.md)            | 予定表グループに新しい予定表を作成します。                    |

## <a name="properties"></a>プロパティ

| プロパティ  | 種類   | 説明                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 名前      | String | グループの名前。                                                                                                                                                                                           |
| changeKey | String | 予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。 |
| classId   | Guid   | クラス識別子。読み取り専用です。                                                                                                                                                                          |
| id        | String | グループの一意識別子。読み取り専用です。                                                                                                                                                                 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                               | 説明                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| 予定表    | [Calendar](calendar.md) collection | 予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
