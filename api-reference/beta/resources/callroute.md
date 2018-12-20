---
title: callRoute リソースの種類
description: CallRoute 型です。
author: VinodRavichandran
ms.openlocfilehash: 9538fb8f27f60e869c19edc7bd19d7f6b29e8fff
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380157"
---
# <a name="callroute-resource-type"></a>callRoute リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

CallRoute 型です。

## <a name="properties"></a>プロパティ

| プロパティ            | 型                          | 説明                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| 最終的な               | [identitySet](identityset.md) | この id は、呼び出しを解決しました。               |
| 翻訳元            | [identitySet](identityset.md) | 呼び出しで使用されていた id です。           |
| routingType         | String                        | 可能な値は、`forwarded`、`lookup`、`selfFork` です。  |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
