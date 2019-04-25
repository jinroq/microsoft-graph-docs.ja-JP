---
title: callroute リソースの種類
description: callroute の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543839"
---
# <a name="callroute-resource-type"></a>callroute リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

callroute の種類。

## <a name="properties"></a>プロパティ

| プロパティ            | 型                          | 説明                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| 最終的な               | [identitySet](identityset.md) | 呼び出しで解決された id。               |
| 翻訳元            | [identitySet](identityset.md) | 最初に呼び出しで使用された id。           |
| routingtype         | String                        | 使用可能な値は、`forwarded`、`lookup`、`selfFork` です。  |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/callroute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
