---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
ms.openlocfilehash: 9d941469da133d9a3e7149dfca55c813f60b3ce8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29579843"
---
# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId リソースの種類

内部使用のみ。

## <a name="json-representation"></a>JSON 表記

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a>プロパティ
| プロパティ         | 型       | 説明
|:-----------------|:-----------|:---------------------
| type             | Int32      | 内部使用のみ。 
| identityProvider | 文字列     | 内部使用のみ。 
| Key              | Edm.Binary | 内部使用のみ。 
