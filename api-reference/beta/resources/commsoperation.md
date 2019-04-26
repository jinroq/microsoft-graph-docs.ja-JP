---
title: commsOperation リソースの種類
description: 長時間実行されている特定の操作の状態。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 34e6ff32c250308e71e05cb5d5c4d04d5671535d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341367"
---
# <a name="commsoperation-resource-type"></a>commsOperation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

長時間実行されている特定の操作の状態。

## <a name="methods"></a>メソッド
なし

## <a name="properties"></a>プロパティ

| プロパティ           | 型                        | 説明                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | String                      | クライアントコンテキスト。                                                             |
| createdDateTime    | DateTimeOffset              | 操作の開始時刻。                                                |
| id                 | String                      | 操作 id。読み取り専用です。 サーバーによって生成されます。                                  |
| lastactiondatetime | DateTimeOffset              | 操作の最後の操作の時刻。                                   |
| resultInfo         | [resultInfo](resultinfo.md) | 結果の情報。 読み取り専用です。 サーバーによって生成されます。                            |
| status             | String                      | 使用可能な値: `notStarted`、`running`、`completed`、`failed`。 読み取り専用。 |

## <a name="relationships"></a>関係
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
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
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
    "@odata.type": "microsoft.graph.resultInfo",
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
  "suppressions": []
}
-->
