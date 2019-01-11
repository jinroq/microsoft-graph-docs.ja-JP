---
title: targetResourceServicePrincipal リソースの種類
description: 監査活動、影響を受けるリソースの ServicePrincipalId を示します。 TargetResource リソースから派生します。
localization_priority: Normal
ms.openlocfilehash: 37bd63851ca9169afb669c710ef4cb2c150ea615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839600"
---
# <a name="targetresourceserviceprincipal-resource-type"></a>targetResourceServicePrincipal リソースの種類
監査活動、影響を受けるリソースの ServicePrincipalId を示します。 [TargetResource](targetresource.md)リソースから派生します。



## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|appId|文字列型 (String)|アプリケーションの一意の Id を示します。 固有のアプリケーションのアプリケーション Id を参照します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
