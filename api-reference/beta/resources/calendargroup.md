---
title: calendarGroup リソースの種類
description: ユーザーの予定表のグループです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cea68da3a91396972c4e237d1fdaf0e16d65e3a3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643714"
---
# <a name="calendargroup-resource-type"></a>calendarGroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| プロパティ  | 型   | 説明                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| name      | String | グループの名前。                                                                                                                                                                                           |
| changeKey | String | 予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。 |
| classId   | Guid   | クラス識別子。読み取り専用です。                                                                                                                                                                          |
| id        | String | グループの一意識別子。読み取り専用です。                                                                                                                                                                 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                               | 説明                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| 予定表    | [Calendar](calendar.md) collection | 予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
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

<!--
{
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/calendargroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
