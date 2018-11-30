---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
ms.openlocfilehash: 067cf88773b5f5d69b2b3538a2ddeab6741631a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066801"
---
# <a name="itemactivitystat-resource-type"></a>itemActivityStat リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
| incompleteData   | [incompleteData][]      | この間隔で統計情報が不完全なデータに基づいていることを示します。 読み取り専用。
| isTrending       | ブール値                 | かどうか、アイテムは「トレンド。」ことを示します。 読み取り専用。
| startDateTime    | DateTimeOffset          | 間隔の開始時。 読み取り専用。
| endDateTime      | DateTimeOffset          | 間隔が終了します。 読み取り専用。
| create           | [itemActionStat][]      | この間隔内のアクションの**作成**についての統計情報です。 読み取り専用。
| edit             | [itemActionStat][]      | この範囲の**編集**処理に関する統計情報です。 読み取り専用。
| delete           | [itemActionStat][]      | この間隔で**削除**の操作に関する統計情報です。 読み取り専用。
| move             | [itemActionStat][]      | この間隔内の**移動**操作に関する統計情報です。 読み取り専用。
| アクセス           | [itemActionStat][]      | この間隔で**のアクセス**の操作に関する統計情報です。 読み取り専用。

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類                        | 説明
|:------------------|:----------------------------|:---------------------------
| アクティビティ        | [itemActivity][] コレクション | この**itemActivityStat**リソースで表される**itemActivities**を公開します。

[itemActivity]: itemactivity.md

## <a name="remarks"></a>解説

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
