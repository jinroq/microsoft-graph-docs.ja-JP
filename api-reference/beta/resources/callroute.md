---
title: callRoute リソースの種類
description: CallRoute の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9978bffd55f62f0646f84d2405df70eba6232d68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974058"
---
# <a name="callroute-resource-type"></a>callRoute リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CallRoute の種類。

## <a name="properties"></a>プロパティ

| プロパティ            | 型                          | 説明                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| 最終的な               | [identitySet](identityset.md) | 呼び出しで解決された id。               |
| 翻訳元            | [identitySet](identityset.md) | 最初に呼び出しで使用された id。           |
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
