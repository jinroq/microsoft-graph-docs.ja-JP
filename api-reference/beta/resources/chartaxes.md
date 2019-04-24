---
title: ChartAxes リソースの種類
description: グラフの軸を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: df18ff1902dd750ef44311e2924a7e63e0ba0e58
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460958"
---
# <a name="chartaxes-resource-type"></a>ChartAxes リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

グラフの軸を表します。


## <a name="methods"></a>メソッド
なし

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|categoryAxis|[ChartAxis](chartaxis.md)|グラフの項目軸を表します。値の取得のみ可能です。|
|系列軸|[ChartAxis](chartaxis.md)|3 次元グラフの系列軸を表します。値の取得のみ可能です。|
|数値軸|[ChartAxis](chartaxis.md)|軸の数値軸を表します。値の取得のみ可能です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
