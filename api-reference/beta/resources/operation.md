---
title: operation リソースの種類
description: 長時間実行されている操作の状態。
localization_priority: Normal
ms.openlocfilehash: e1e0f7a886d460bc378fdc75041e17b997897e2d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341785"
---
# <a name="operation-resource-type"></a>operation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

長時間実行されている操作の状態。

## <a name="methods"></a>メソッド

なし

## <a name="properties"></a>プロパティ

| プロパティ           | 型            | 説明                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| createdDateTime    | DateTimeOffset  | 操作の開始時刻。                                                |
| id                 | String          | 操作 id。読み取り専用です。 サーバーによって生成されます。                                  |
| lastactiondatetime | DateTimeOffset  | 操作の最後の操作の時刻。                                   |
| status             | String          | 使用可能な値: `notStarted`、`running`、`completed`、`failed`。 読み取り専用です。 |

## <a name="relationships"></a>関係

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
