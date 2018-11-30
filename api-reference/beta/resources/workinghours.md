---
title: workingHours リソースの種類
description: ユーザーが働く曜日と、特定のタイムゾーンの時間を表します。
ms.openlocfilehash: 915ec185931d3f7e77f010517a3ef0c3bff92204
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071906"
---
# <a name="workinghours-resource-type"></a>workingHours リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザーが働く曜日と、特定のタイムゾーンの時間を表します。

アクティビティまたはリソースの計画に対処するシナリオでは、ユーザーの就業時間にアクセスできると便利です。 ユーザーの就業時間は、ユーザーの[メールボックス設定](mailboxsettings.md)の一部として[取得](../api/user-get-mailboxsettings.md#request-3)、[設定](../api/user-update-mailboxsettings.md#request-2)できます。 

就業時間には、Outlook クライアントに設定したタイム ゾーンとは異なるタイム ゾーンを設定できます。 これは、通常の勤務地とは異なるタイム ゾーンに移動する場合に役立ちます。 Outlook クライアントを  
移動先のタイム ゾーンに設定すると、現地にいる間、Outlook の時刻の値を現地時間で表示できます。
他のユーザーが通常の勤務地での時間で会議を要求するとしても、該当するタイム ゾーンでの就業時間が考慮されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| daysOfWeek | String コレクション | ユーザーが働く曜日。 |
| startTime | Edm.TimeOfDay | ユーザーの始業時間。 |
| endTime | Edm.TimeOfDay | ユーザーの終業時間。 |
| timeZone | [timeZoneBase](timezonebase.md) | 就業時間に適用するタイム ゾーン。 |


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->