---
title: plannerAppliedCategories リソースの種類
description: '**AppliedCategoriesCollection**リソースは、タスクに適用されている項目 (またはラベル) のコレクションを表します。 PlannerTask オブジェクトの一部です。'
localization_priority: Normal
ms.openlocfilehash: a47317f907b8ee934a59a320af67e94ce6d3bf8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856015"
---
# <a name="plannerappliedcategories-resource-type"></a>plannerAppliedCategories リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**AppliedCategoriesCollection** リソースは、タスクに適用されているカテゴリ (またはラベル) のコレクションを表します。これは [plannerTask](plannertask.md) オブジェクトの一部です。最大 6 つのカテゴリをタスクに適用できます。カテゴリの説明 (`category1`、`category2` など) は、[計画の詳細](plannerplandetails.md)オブジェクトの一部です。これはオープン型です。

## <a name="properties"></a>プロパティ
クライアントは、オープン型のプロパティを定義できます。ただし、この場合クライアントは、対応するカテゴリがタスクに適用される際に、`category1`、`category2`、`category3`、`category4`、`category5` および/または `category6` を、`true` ブール値が設定されたプロパティとして指定する必要があります。以下に例を示します。これらが適用されなくなると、プロパティはその値が `false` ブール値に設定され、自動的に削除されます。 

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
