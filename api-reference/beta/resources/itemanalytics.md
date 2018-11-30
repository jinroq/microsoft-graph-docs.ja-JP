---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
ms.openlocfilehash: b50df7d1fdf67cffd508c3b5891d07c599521c8a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068821"
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

| プロパティ      | 型                 | 説明
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
