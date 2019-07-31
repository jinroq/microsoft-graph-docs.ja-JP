---
title: governancePermission リソースの種類
description: 'GovernanceSubject が特定の governanceResource に対して持つアクセス許可を表します。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8bf32b855ed77ccdf712b1a739ef913d0a3dade0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971944"
---
# <a name="governancepermission-resource-type"></a>governancePermission リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[GovernanceSubject](../resources/governancesubject.md)が特定の[governanceResource](../resources/governanceresource.md)に対して持つアクセス許可を表します。  


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
