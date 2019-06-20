---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。 今後、この複合型は廃止されます。
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/20/2019
ms.locfileid: "35083943"
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
