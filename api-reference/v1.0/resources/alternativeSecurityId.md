---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d4cdfa609e5cc2daf484bf0f35b863285ee811dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033244"
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
