---
title: followupFlag リソースの種類
description: 'ユーザーが後でフォローするためのアイテムにフラグを設定できます。 '
ms.openlocfilehash: 5aa9d82fc90d7142717ac5ef05f9d837bac371ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023767"
---
# <a name="followupflag-resource-type"></a>followupFlag リソースの種類


ユーザーが後でフォローするためのアイテムにフラグを設定できます。 

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|CompletedDateTime|[dateTimeTimeZone](datetimetimezone.md)|フォローアップが終了した日時。|
|dueDateTime|**dateTimeTimeZone**|フォローアップが終了する予定の日時。|
|FlagStatus|followupFlagStatus|アイテムのフォローアップ状態。 可能な値は、`notFlagged`、`complete`、`flagged` です。|
|startDateTime|**dateTimeTimeZone**|フォローアップを開始する予定の日時。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
