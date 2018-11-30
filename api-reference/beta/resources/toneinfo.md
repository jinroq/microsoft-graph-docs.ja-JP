---
title: toneInfo リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: b4ed9667c2e2156f52703c6fa15f4937ead5cef4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073773"
---
# <a name="toneinfo-resource-type"></a>toneInfo リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

## <a name="properties"></a>プロパティ

| プロパティ       | 型    | 説明|
|:---------------|:--------|:----------|
| sequenceId | Int64 | DTMF イベントの順序付けに使用される増分の識別子です。 |
| トーン | String | 使用可能な値: `tone0`、 `tone1`、 `tone2`、 `tone3`、 `tone4`、 `tone5`、 `tone6`、 `tone7`、 `tone8`、 `tone9`、 `star`、 `pound`、 `a`、 `b`、 `c`、 `d`、 `flash`。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->