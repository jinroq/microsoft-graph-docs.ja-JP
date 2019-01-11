---
title: assignedLicense リソースの種類
description: ユーザーに割り当てられているライセンスを表します。ユーザー エンティティの **assignedLicenses** プロパティは、**assignedLicense** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 1e190060d0aafa4d494240f691b354b28e7697c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885345"
---
# <a name="assignedlicense-resource-type"></a>assignedLicense リソースの種類

ユーザーに割り当てられているライセンスを表します。[ユーザー](user.md) エンティティの **assignedLicenses** プロパティは、**assignedLicense** のコレクションです。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
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
