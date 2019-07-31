---
author: daspek
description: Itemactivit(リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。
ms.date: 09/14/2017
title: Itemactiv
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61c410d807869615ed35365743d1ae87b5b6e890
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967100"
---
# <a name="itemactivitystat-resource-type"></a>リソースの種類での itemactiv

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Itemactivit(** リソース) は、ある期間内に発生したアクティビティに関する情報を提供します。

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
