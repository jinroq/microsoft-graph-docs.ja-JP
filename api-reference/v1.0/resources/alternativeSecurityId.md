---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569481"
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
| type             | Int32      | システム内部でのみ使用します。
| identityProvider | string     | システム内部でのみ使用します。
| キー              | Edm。バイナリ | システム内部でのみ使用します。
