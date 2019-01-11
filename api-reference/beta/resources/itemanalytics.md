---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 03626b5dad041181558af076b5dc0ac05b684e13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842414"
---
# <a name="itemanalytics-resource-type"></a>itemAnalytics リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**ItemAnalytics**リソースでは、アイテムに対して行われたアクティビティに関する分析を提供します。 このリソースは、現在 SharePoint およびビジネスのための OneDrive で使用可能なのみです。

間隔またはユーザー設定の時刻の範囲の上で分析を取得するために、 [getActivitiesByInterval][] API を使用することもできます。

>**注:****ItemAnalytics**リソースはまだすべての[国内展開](/graph/deployments)で使用可能ではありません。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```

## <a name="properties"></a>プロパティ

| プロパティ      | 種類                 | 説明
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | 分析で、アイテムの有効期間です。
| lastSevenDays | [itemActivityStat][] | 過去 7 日間の分析。

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->
