---
title: rankedEmailAddress リソースの種類
description: ランクの電子メール アドレスを表します。
ms.openlocfilehash: 9234f527ecba6dc83f2e4f80911442d4a083503a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073313"
---
# <a name="rankedemailaddress-resource-type"></a>rankedEmailAddress リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ランクの電子メール アドレスを表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|address|文字列|電子メール アドレス。|
|rank|double|電子メール アドレスのランキングです。 ランクは、他の返される結果に関連して、並べ替えキーとして使用されます。 上位の値は、関連性の高い結果に対応します。 関連性は、通信、コラボレーション、取引関係のシグナルによって決定されます。|

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
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
