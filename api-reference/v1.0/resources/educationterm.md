---
title: educationTerm リソースの種類
description: 用語。 これは学年度の指定された部分を示します。 educationClass 内で使用します。
author: mmast-msft
ms.openlocfilehash: 319eedbaebde4f1e76c2f1b3e124c0dad2642538
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353089"
---
# <a name="educationterm-resource-type"></a>educationTerm リソースの種類

用語。 これは学年度の指定された部分を示します。 [educationClass](educationclass.md) 内で使用します。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|displayName| String| 用語の表示名。| 
|externalId|String| 同期システム内の用語の ID。|
|startDate|Date|用語の開始。|
|endDate|Date|用語の終了。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->