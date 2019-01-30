---
title: commsOperation リソースの種類
description: 特定の実行時間の長い操作のステータス。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b7914bd9692b4d9a94294f9a09659467e10550a6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642206"
---
# <a name="commsoperation-resource-type"></a>commsOperation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定の実行時間の長い操作のステータス。

## <a name="methods"></a>メソッド
なし

## <a name="properties"></a>プロパティ

| プロパティ           | 型                        | 説明                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | String                      | クライアントのコンテキスト。                                                             |
| createdDateTime    | DateTimeOffset              | 操作の開始時刻です。                                                |
| id                 | String                      | 操作 ID です。読み取り専用です。 サーバーによって生成されます。                                  |
| lastActionDateTime | DateTimeOffset              | 操作の最後の操作の時間です。                                   |
| resultInfo         | [resultInfo](resultinfo.md) | 結果の情報。 読み取り専用です。 サーバーによって生成されます。                            |
| status             | String                      | 使用可能な値: `notStarted`、`running`、`completed`、`failed`。 読み取り専用です。 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "#microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
