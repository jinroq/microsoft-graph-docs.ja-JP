---
title: updateWindow リソースの種類
description: updateWindow リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 57fb977dd853261300ed09dd8d9b3c343f62bea0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840955"
---
# <a name="updatewindow-resource-type"></a>updateWindow リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[エージェント](onpremisesagent.md)が更新を受信できる時間枠を表します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|updateWindowEndTime|TimeOfDay|エージェントが更新を受信できる時間枠の終わり|
|updateWindowStartTime|TimeOfDay|エージェントが更新プログラムを受信できる時間枠の開始|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateWindow",
  "baseType": null
}-->

```json
{
  "updateWindowEndTime": "String (timestamp)",
  "updateWindowStartTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "updateWindow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
