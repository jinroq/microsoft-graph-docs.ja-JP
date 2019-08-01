---
author: daspek
ms.author: dspektor
title: リソースの種類での itemactiv
description: Itemactivitのオブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bf4396e6da5c56b19d33d7a914d864cb6dd54592
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036674"
---
# <a name="itemactivitystat-resource-type"></a>リソースの種類での itemactiv

**Itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。

## <a name="properties"></a>プロパティ

| プロパティ         | 型                    | 説明
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | この間隔の統計情報が不完全なデータに基づくことを示します。 読み取り専用です。
| isTrending       | Boolean                 | アイテムが "傾向" であるかどうかを示します。 読み取り専用です。
| startDateTime    | DateTimeOffset          | 間隔が開始されたとき。 読み取り専用です。
| endDateTime      | DateTimeOffset          | 間隔が終了したとき。 読み取り専用です。
| create           | [itemActionStat][]      | この間隔における**create**アクションに関する統計。 読み取り専用です。
| edit             | [itemActionStat][]      | この間隔の**編集**アクションに関する統計。 読み取り専用です。
| delete           | [itemActionStat][]      | この間隔の**削除**アクションに関する統計情報。 読み取り専用です。
| move             | [itemActionStat][]      | この間隔における**移動**アクションに関する統計。 読み取り専用です。
| 接続           | [itemActionStat][]      | この間隔における**アクセス**アクションに関する統計情報。 読み取り専用です。

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類                        | 説明
|:------------------|:----------------------------|:---------------------------
| アクティビティ        | [itemActivity][] コレクション | この**Itemactivitの**リソースで表された**itemactivities**を公開します。

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
