---
title: rankedEmailAddress リソースの種類
description: ランク付けされた電子メールアドレスを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e29d5b2f2116050f9cea036df35ed6cc012c0e36
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965524"
---
# <a name="rankedemailaddress-resource-type"></a>rankedEmailAddress リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ランク付けされた電子メールアドレスを表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|address|string|電子メール アドレス。|
|rank|double|電子メールアドレスのランク。 ランクは、他の返された結果に対して並べ替えキーとして使用されます。 上位の値は、関連性の高い結果に対応します。 関連性は、通信、コラボレーション、取引関係のシグナルによって決定されます。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
