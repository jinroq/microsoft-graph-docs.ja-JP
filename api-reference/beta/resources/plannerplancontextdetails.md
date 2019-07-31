---
title: プラン、Contextdetails リソースの種類
description: 「 **Plan The Contextdetails** resource」には、プランのコンテキストに関する追加情報が含まれています。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9d4bf7d0a5c2149f826097eedc350e81eb32bf70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009021"
---
# <a name="plannerplancontextdetails-resource-type"></a>プラン、Contextdetails リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

「 **Plan The Contextdetails** resource」には、プランの[コンテキスト](plannerplancontext.md)に関する追加情報が含まれています。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|url|String|関連する[プランのコンテキスト](plannerplancontext.md)によって表されるユーザーの作業の URL。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
