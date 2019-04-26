---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
localization_priority: Normal
ms.openlocfilehash: 60e45c6d914c64f92b9f15f78fda22372a23e91f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345842"
---
# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId リソースの種類

内部使用のみ。 今後、この複合型は廃止されます。

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
| type             | Int32      | システム内部でのみ使用します。
| identityProvider | string     | システム内部でのみ使用します。
| キー              | Edm。バイナリ | システム内部でのみ使用します。
