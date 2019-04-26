---
title: resourceReference リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: accd2b0b12f8068ea990fbd611b46053f66d6de4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340003"
---
# <a name="resourcereference-resource-type"></a>resourceReference リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[insights](officegraphinsights.md)のプロパティを含む複合型。

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
| id            | String    | アイテムの一意の識別子。           |
| type          | String    | アイテムの分類に使用できる文字列値 ("microsoft....." など) |
