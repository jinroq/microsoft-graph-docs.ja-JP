---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemactiv
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561909"
---
# <a name="itemactivitystat-resource-type"></a>リソースの種類での itemactiv

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。

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
| incompletedata   | [incompletedata][]      | この間隔の統計情報が不完全なデータに基づくことを示します。 読み取り専用。
| istrending       | Boolean                 | アイテムが "傾向" であるかどうかを示します。 読み取り専用。
| startDateTime    | DateTimeOffset          | 間隔が開始されたとき。 読み取り専用。
| endDateTime      | DateTimeOffset          | 間隔が終了したとき。 読み取り専用。
| create           | [itemactionstat][]      | この間隔における**create**アクションに関する統計。 読み取り専用。
| edit             | [itemactionstat][]      | この間隔の**編集**アクションに関する統計。 読み取り専用。
| delete           | [itemactionstat][]      | この間隔の**削除**アクションに関する統計情報。 読み取り専用。
| move             | [itemactionstat][]      | この間隔における**移動**アクションに関する統計。 読み取り専用。
| 接続           | [itemactionstat][]      | この間隔における**アクセス**アクションに関する統計情報。 読み取り専用。

[itemactionstat]: itemactionstat.md
[incompletedata]: incompletedata.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類                        | 説明
|:------------------|:----------------------------|:---------------------------
| アクティビティ        | [itemActivity][] コレクション | この**itemactivitの**リソースで表された**itemactivities**を公開します。

[itemActivity]: itemactivity.md

## <a name="remarks"></a>備考

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
