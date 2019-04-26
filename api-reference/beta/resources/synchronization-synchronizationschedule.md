---
title: 同期スケジュールリソースの種類
description: 同期ジョブの実行に使用されるスケジュールを定義します。
localization_priority: Normal
ms.openlocfilehash: 2ae5473463e84fdf27882df1b243049cc98ab043
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340048"
---
# <a name="synchronizationschedule-resource-type"></a>同期スケジュールリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[同期ジョブ](synchronization-synchronizationjob.md)の実行に使用されるスケジュールを定義します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|nntp|DateTimeOffset|このジョブの有効期限が切れる日付と時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|interval|期間|同期の反復間の間隔。|
|state|String| 使用可能な値は、`Active`、`Disabled` です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
