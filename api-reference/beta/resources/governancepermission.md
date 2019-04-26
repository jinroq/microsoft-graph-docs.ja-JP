---
title: governancePermission リソースの種類
description: 'governanceSubject が特定の governanceResource に対して持つアクセス許可を表します。  '
localization_priority: Normal
ms.openlocfilehash: 2f6be4bdc502f829b1dcfd991d1c2ae6130dea8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340183"
---
# <a name="governancepermission-resource-type"></a>governancePermission リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[governanceSubject](../resources/governancesubject.md)が特定の[governanceResource](../resources/governanceresource.md)に対して持つアクセス許可を表します。  


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accessLevel|String|アクセスレベル。 有効な値``None``は``UserRead``、 ``AdminRead``、、 ``AdminReadWrite``、です。|
|isActive|Boolean|要求者がアクセスレベルに対してアクティブなロール割り当てを持っているかどうかを示します。|
|isEligible|Boolean|要求者がアクセスレベルに対して適格な役割の割り当てを持っているかどうかを示します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
