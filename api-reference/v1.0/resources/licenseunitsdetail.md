---
title: licenseUnitsDetail リソースの種類
description: '**subscribedSku** エンティティの prepaidUnits のプロパティは、**licenseUnitsDetail** 型です。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b4540cb546c8dae9d519a68b6ace8d030b6c40cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036464"
---
# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail リソースの種類

**subscribedSku** エンティティの [prepaidUnits](subscribedsku.md) のプロパティは、**licenseUnitsDetail** 型です。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:-------------|:-----|:----------|
|enabled|Int32| 有効になっている単位の数。 |
|suspended|Int32| 中断されている単位の数。 |
|warning|Int32| 警告状態にある単位数。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
