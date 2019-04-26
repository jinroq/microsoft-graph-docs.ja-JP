---
title: callroute リソースの種類
description: callroute の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06dd1a2265c5a6bda9feba0b51e7fd731d7945c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328278"
---
# <a name="callroute-resource-type"></a>callroute リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

callroute の種類。

## <a name="properties"></a>プロパティ

| プロパティ            | 型                          | 説明                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| 最終的な               | [identitySet](identityset.md) | 呼び出しで解決された id。               |
| 翻訳元            | [identitySet](identityset.md) | 最初に呼び出しで使用された id。           |
| routingtype         | String                        | 可能な値は、`forwarded`、`lookup`、`selfFork` です。  |

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
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
