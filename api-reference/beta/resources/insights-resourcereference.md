---
title: resourceReference リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 06a8d99ba01a8a3fd3d171b800345f81b0819de0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005724"
---
# <a name="resourcereference-resource-type"></a>resourceReference リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Insights](officegraphinsights.md)のプロパティを含む複合型。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明  |
| ------------- |-----------| -------------|
| webUrl        | String    | 参照されるアイテムにつながる URL。 |
| id            | 文字列    | アイテムの一意の識別子。           |
| type          | String    | アイテムの分類に使用できる文字列値 ("microsoft....." など) |
