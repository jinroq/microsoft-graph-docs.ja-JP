---
title: タイムスタンプのリソースの種類
description: 時間のポイントの日付と時刻情報です。
ms.openlocfilehash: 24326f0c104dd4ee2be80016ce798cc843288975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070015"
---
# <a name="timestamp-resource-type"></a>タイムスタンプのリソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

時間のポイントの日付と時刻情報です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|date|日付|タイムスタンプの日付部分。|
|time|TimeOfDay|タイムスタンプの時刻部分。|
|timeZone|String|タイムスタンプは、世界中の 24 の前後の領域の 1 つのタイム ゾーンの部分です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->