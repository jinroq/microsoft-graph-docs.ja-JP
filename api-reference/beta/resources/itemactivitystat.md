---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemactiv
localization_priority: Normal
ms.openlocfilehash: 08bbfd414a32e8eb8a0144d879ede55c71c19b89
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339882"
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
| incompletedata   | [incompletedata][]      | この間隔の統計情報が不完全なデータに基づくことを示します。 読み取り専用です。
| istrending       | Boolean                 | アイテムが "傾向" であるかどうかを示します。 読み取り専用です。
| startDateTime    | DateTimeOffset          | 間隔が開始されたとき。 読み取り専用です。
| endDateTime      | DateTimeOffset          | 間隔が終了したとき。 読み取り専用です。
| create           | [itemactionstat][]      | この間隔における**create**アクションに関する統計。 読み取り専用です。
| edit             | [itemactionstat][]      | この間隔の**編集**アクションに関する統計。 読み取り専用です。
| delete           | [itemactionstat][]      | この間隔の**削除**アクションに関する統計情報。 読み取り専用です。
| move             | [itemactionstat][]      | この間隔における**移動**アクションに関する統計。 読み取り専用です。
| 接続           | [itemactionstat][]      | この間隔における**アクセス**アクションに関する統計情報。 読み取り専用です。

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
  "suppressions": []
}
-->
