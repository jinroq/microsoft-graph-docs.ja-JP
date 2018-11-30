---
title: licenseUnitsDetail リソースの種類
description: subscribedSku エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。
ms.openlocfilehash: e8cf5253676dab8a4b31c3ab33faa0af3ddfd527
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020381"
---
# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail リソースの種類

[subscribedSku](subscribedsku.md) エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:-------------|:-----|:----------|
|enabled|Int32| 有効になっている単位の数です。 |
|suspended|Int32| 利用停止中の単位の数です。 |
|warning|Int32| 警告ステータスのユニットの数です。 |

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
