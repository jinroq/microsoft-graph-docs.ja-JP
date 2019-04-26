---
title: プランリソースの種類
description: /**コレクション**リソースは、タスクに適用されているカテゴリ (またはラベル) のコレクションを表します。 このメソッドは、プランのタスクオブジェクトに含まれています。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a927adb78bc0fe1c5135281043ecbdd3afe09a60
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344625"
---
# <a name="plannerappliedcategories-resource-type"></a>プランリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

/**コレクション**リソースは、タスクに適用されているカテゴリ (またはラベル) のコレクションを表します。 このメソッドは、[プランのタスク](plannertask.md)オブジェクトに含まれています。
1つのタスクには最大6つのカテゴリを適用できます。 カテゴリの説明 ( `category1` `category2`など) は、 [plan details](plannerplandetails.md)オブジェクトの一部です。 これはオープン型です。

## <a name="properties"></a>プロパティ
オープン型のプロパティは、クライアントで定義できます。 この場合、クライアントは、対応するカテゴリ`category1`が`category2`タスク`category3`に`category4`適用`category5`されるとき`category6`に`true`ブール値で、、、、および/またはをプロパティとしてプロパティとして提供する必要があります。 例を以下に示します。 このプロパティが適用されていない場合、プロパティの値を`false` boolean に設定すると、プロパティが自動的に削除されます。 

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

例: 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
