---
title: assignedLicense リソースの種類
description: ユーザーに割り当てられているライセンスを表します。 User エンティティの**assignedLicenses**プロパティは、 **assignedLicense**のコレクションです。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cd551085dac72b2f63e2cb67d9ada978746c0b5c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030080"
---
# <a name="assignedlicense-resource-type"></a>assignedLicense リソースの種類

ユーザーに割り当てられているライセンスを表します。 [User](user.md)エンティティの**assignedLicenses**プロパティは、 **assignedLicense**のコレクションです。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|disabledPlans|Guid コレクション|無効になっているプランの一意識別子のコレクション。|
|skuId|Guid|SKU の一意識別子。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
