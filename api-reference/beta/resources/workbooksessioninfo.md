---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
ms.openlocfilehash: c04afe17c10edd8b136465d6d7ae3dbedb6307ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069828"
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

| プロパティ | 型  | 説明                               |
|:---------|:------|:------------------------------------------|
| ID  | 文字列 | ブック セッションの ID。 |
| persistChanges | 文字列 |  `true`: 永続セッションの場合。 `false`: 非永続セッション (表示モード) の場合。 |

