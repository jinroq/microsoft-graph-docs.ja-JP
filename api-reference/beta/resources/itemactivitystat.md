---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517632"
---
# <a name="itemactivitystat-resource-type"></a>itemActivityStat リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemActivityStat**リソースでは、時間間隔内で行われた活動についての情報を提供します。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

## <a name="properties"></a>プロパティ

| プロパティ         | 型                    | 説明
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | この間隔で統計情報が不完全なデータに基づいていることを示します。 読み取り専用です。
| isTrending       | ブール値                 | かどうか、アイテムは「トレンド。」ことを示します。 読み取り専用です。
| startDateTime    | DateTimeOffset          | 間隔の開始時。 読み取り専用です。
| endDateTime      | DateTimeOffset          | 間隔が終了します。 読み取り専用です。
| create           | [itemActionStat][]      | この間隔内のアクションの**作成**についての統計情報です。 読み取り専用です。
| edit             | [itemActionStat][]      | この範囲の**編集**処理に関する統計情報です。 読み取り専用です。
| delete           | [itemActionStat][]      | この間隔で**削除**の操作に関する統計情報です。 読み取り専用です。
| move             | [itemActionStat][]      | この間隔内の**移動**操作に関する統計情報です。 読み取り専用です。
| Access           | [itemActionStat][]      | この間隔で**のアクセス**の操作に関する統計情報です。 読み取り専用です。

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類                        | 説明
|:------------------|:----------------------------|:---------------------------
| アクティビティ        | [itemActivity][] コレクション | この**itemActivityStat**リソースで表される**itemActivities**を公開します。

[itemActivity]: itemactivity.md

## <a name="remarks"></a>解説

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
