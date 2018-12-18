---
title: ChartAxisTitleFormat リソースの種類
description: グラフ軸のタイトルの書式設定を表します。
author: lumine2008
ms.openlocfilehash: 7a160f02f06c74edeee09f91b2b117ea437291e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343023"
---
# <a name="chartaxistitleformat-resource-type"></a>ChartAxisTitleFormat リソースの種類

グラフ軸のタイトルの書式設定を表します。


## <a name="methods"></a>メソッド
なし

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|font|[WorkbookChartFont](chartfont.md)|グラフの軸タイトルのオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->