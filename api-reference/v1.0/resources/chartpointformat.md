---
title: ChartPointFormat リソースの種類
description: グラフのポイントのオブジェクトの書式設定を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c1b0a4a7d9076771da11061723f275079d429cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569068"
---
# <a name="chartpointformat-resource-type"></a>ChartPointFormat リソースの種類

グラフのポイントのオブジェクトの書式設定を表します。


## <a name="methods"></a>メソッド
なし

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|背景の書式設定情報を含むグラフの塗りつぶしの書式を表します。 読み取り専用。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
