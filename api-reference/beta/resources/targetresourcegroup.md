---
title: targetResourceGroup リソースの種類
description: '監査活動により影響を受けたグループの種類を示します。 Azure AD と統合されたグループと同じように値が含まれています '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069756"
---
# <a name="targetresourcegroup-resource-type"></a>targetResourceGroup リソースの種類
監査活動により影響を受けたグループの種類を示します。 Azure AD と統合されたグループと同じように値が含まれています 



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|groupType|String| 可能な値は、`unifiedGroups`、`azureAD`、`unknownFutureValue` です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->