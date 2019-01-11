---
title: scheduleItem のリソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: e5d14826a27153af27648484554ec864d62ed6c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890434"
---
# <a name="scheduleitem-resource-type"></a>scheduleItem のリソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
ユーザーの既定の予定表に、実際のイベントに対応するユーザーの可用性を説明する項目です。 リソースも同様にこの項目が適用されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |日付、時刻、およびタイム ゾーンに対応するイベントが終了します。 |
|isPrivate |ブール型 |対応するイベントの重大度。 イベントが設定されている場合は true。`private`は false、それ以外の場合。 |
|location |String | 場所の対応するイベントが保持されているから参加します。 省略可能。|
|start |[dateTimeTimeZone](datetimetimezone.md) |日付、時刻、およびタイム ゾーンに対応するイベントが開始します。 |
|status |String | ユーザーまたは対応するイベントの中にリソースの可用性の状態です。 可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。 |
|subject |String | 対応するイベントの件名の行です。 省略可能。|


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
