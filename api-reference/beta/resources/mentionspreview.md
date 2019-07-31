---
title: mentionsPreview リソースの種類
description: リソースインスタンス内のメンションオブジェクトに関する情報を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5c4604657e18498a85aa8646b5d69db7d74299bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009707"
---
# <a name="mentionspreview-resource-type"></a>mentionsPreview リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

リソースインスタンス内の[メンション](../resources/mention.md)オブジェクトに関する情報を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| 説明 | Boolean | True の場合は、サインインしているユーザーが親リソースインスタンスで言及されます。 読み取り専用です。 フィルターをサポートします。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
