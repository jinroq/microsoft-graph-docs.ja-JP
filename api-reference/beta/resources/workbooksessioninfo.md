---
title: workbookSessionInfo リソース型
description: ブック セッションについての情報を提供します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3b2d52b6389c6fc00eb0bf3b3b6d81774f6f882a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963914"
---
# <a name="workbooksessioninfo-resource-type"></a>workbookSessionInfo リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| id  | string | ブック セッションの ID。 |
| persistChanges | string |  `true`: 永続セッションの場合。 `false`: 非永続セッション (表示モード) の場合。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookSessionInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
