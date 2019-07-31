---
title: プラン? カテゴリの説明リソースの種類
description: 'プラン**** に対して定義されているカテゴリの説明的なラベルを表します。 プランの詳細オブジェクトに属します。 最大6つのカテゴリが定義されています。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a8d80be1768cae3383b07c6fbb7dac1e042cc0bd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966026"
---
# <a name="plannercategorydescriptions-resource-type"></a>プラン? カテゴリの説明リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プラン**** に対して定義されているカテゴリの説明的なラベルを表します。 [プランの詳細](plannerplandetails.md)オブジェクトに属します。 最大6つのカテゴリが定義されています。 


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|category1|String|カテゴリ1に関連付けられているラベル|
|category2|String|カテゴリ2に関連付けられているラベル|
|category3|String|カテゴリ3に関連付けられているラベル|
|category4|String|Category 4 に関連付けられているラベル|
|category5|String|カテゴリ5に関連付けられているラベル|
|category6|String|カテゴリ6に関連付けられているラベル|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
