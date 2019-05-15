---
author: daspek
ms.author: dspektor
title: リソースの種類での itemactiv
description: Itemactivitのオブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3af10bba565585341d04cdc47702e18e71d8accd
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970760"
---
# <a name="itemactivitystat-resource-type"></a>リソースの種類での itemactiv

**Itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。

## <a name="properties"></a>プロパティ

| プロパティ         | 型                    | 説明
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | この間隔の統計情報が不完全なデータに基づくことを示します。 値の取得のみ可能です。
| isTrending       | Boolean                 | アイテムが "傾向" であるかどうかを示します。 値の取得のみ可能です。
| startDateTime    | DateTimeOffset          | 間隔が開始されたとき。 値の取得のみ可能です。
| endDateTime      | DateTimeOffset          | 間隔が終了したとき。 値の取得のみ可能です。
| create           | [itemActionStat][]      | この間隔における**create**アクションに関する統計。 値の取得のみ可能です。
| edit             | [itemActionStat][]      | この間隔の**編集**アクションに関する統計。 値の取得のみ可能です。
| delete           | [itemActionStat][]      | この間隔の**削除**アクションに関する統計情報。 値の取得のみ可能です。
| move             | [itemActionStat][]      | この間隔における**移動**アクションに関する統計。 値の取得のみ可能です。
| 接続           | [itemActionStat][]      | この間隔における**アクセス**アクションに関する統計情報。 値の取得のみ可能です。

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類                        | 説明
|:------------------|:----------------------------|:---------------------------
| アクティビティ        | [itemActivity][] コレクション | この**Itemactivitの**リソースで表された**Itemactivities**を公開します。

[itemActivity]: itemactivity.md

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
