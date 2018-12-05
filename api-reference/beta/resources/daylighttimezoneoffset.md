---
title: daylightTimeZoneOffset リソースの種類
description: タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。
ms.openlocfilehash: 1504a3c1bb1b2d6c691aadf1d073a95453f76d2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066859"
---
# <a name="daylighttimezoneoffset-resource-type"></a>daylightTimeZoneOffset リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。

たとえば、タイム ゾーンに次のプロパティが指定されているとします。

- **bias**: 300
- **daylightBias**: -100
- **dayOccurrence**: 4
- **dayOfWeek**: "日曜日"
- **month**: 5
- **time** は 02:00:00 で、_ **year** は 0 です。つまり、夏時間の間は、時刻が UTC より +300-100=200 分進んでいることを意味します。 夏時間から標準時への切り替えは、毎年 5 月の第 4 日曜日の午前 2 時に行われます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| daylightBias | Edm.Int32 | 夏時間の協定世界時 (UTC) からの時間オフセットです。 この値は分単位です。  |
| dayOccurrence | Edm.Int32 | 標準時から夏時間への切り替えが月の何番目の曜日に行われるかを表します。 |
| dayOfWeek | 文字列 | 標準時から夏時間への切り替えが行われる曜日を表します。 |
| month | Edm.Int32 | 標準時から夏時間への切り替えが行われる月を表します。 |
| time | Edm.TimeOfDay | 標準時から夏時間への切り替えが行われる時刻を表します。 |
| year | Edm.Int32 | 標準時から夏時間への切り替えが年に何回行われるかを表します。 たとえば、値 0 は年に 1 回を意味します。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->