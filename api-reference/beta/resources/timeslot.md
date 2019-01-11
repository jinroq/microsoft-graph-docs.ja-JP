---
title: timeSlot リソースの種類
description: 期間です。
localization_priority: Normal
ms.openlocfilehash: 1f383a7feafbb3816ef838d8f0667eebdd42443f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877932"
---
# <a name="timeslot-resource-type"></a>timeSlot リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

期間です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|end|[dateTimeTimeZone](datetimetimezone.md)|期間の開始時間。|
|start|[dateTimeTimeZone](datetimetimezone.md)|期間の終了時間。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
