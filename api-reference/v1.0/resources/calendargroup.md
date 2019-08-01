---
title: calendarGroup リソースの種類
description: ユーザーカレンダーのグループ。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3931359b3b7eec65e2c675fbc5b6ef40176b13fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033055"
---
# <a name="calendargroup-resource-type"></a>calendarGroup リソースの種類

ユーザーカレンダーのグループ。

## <a name="methods"></a>メソッド

| メソッド                                                      | 戻り値の型                        | 説明                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [予定表グループを一覧表示する](../api/user-list-calendargroups.md)  | [Calendar](calendar.md) コレクション | ユーザーの予定表グループを取得します。                               |
| [予定表グループを作成する](../api/user-post-calendargroups.md) | [Calendar](calendar.md)            | 新しい予定表グループを作成します。                                  |
| [予定表グループを取得する](../api/calendargroup-get.md)           | [calendarGroup](calendargroup.md)  | 予定表グループ オブジェクトのプロパティと関係を読み取ります。 |
| [Update](../api/calendargroup-update.md)                    | [calendarGroup](calendargroup.md)  | calendarGroup オブジェクトを更新します。                                  |
| [Delete](../api/calendargroup-delete.md)                    | None                               | calendarGroup オブジェクトを削除します。                                  |
| [List calendars](../api/calendargroup-list-calendars.md)    | [Calendar](calendar.md) collection | 予定表グループ内の予定表を一覧表示する                           |
| [予定表を作成する](../api/calendargroup-post-calendars.md)   | [Calendar](calendar.md)            | 予定表グループに新しい予定表を作成します。                    |

## <a name="properties"></a>プロパティ

| プロパティ  | 型   | 説明                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| name      | String | グループの名前。                                                                                                                                                                                           |
| changeKey | String | 予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。 |
| classId   | Guid   | クラス識別子。読み取り専用です。                                                                                                                                                                          |
| id        | String | グループの一意識別子。読み取り専用です。                                                                                                                                                                 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                               | 説明                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| calendars    | [Calendar](calendar.md) collection | 予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。 |

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
