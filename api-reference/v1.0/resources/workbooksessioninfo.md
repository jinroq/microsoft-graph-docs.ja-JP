---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 900ebdcefbdfa83e7b72b1c926a441f1c497626a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826930"
---
# <a name="workbooksessioninfo-resource-type"></a>workbookSessionInfo リソース型

ブック セッションについての情報を提供します。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 種類  | 説明                               |
|:---------|:------|:------------------------------------------|
| ID  | 文字列 | ブック セッションの ID。 |
| persistChanges | ブール |  `true`: 永続セッションの場合。 `false`: 非永続セッション (表示モード) の場合。 |

