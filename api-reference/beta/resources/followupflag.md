---
title: followupFlag リソースの種類
description: ユーザーが特定のアイテムを後でフォローアップできるよう、フラグを設定できます。 サポートされているアイテムには、メッセージと連絡先があります。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28f60187fcfb3d41779547b6252edf69c1fc2735
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971978"
---
# <a name="followupflag-resource-type"></a>followupFlag リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーが特定のアイテムを後でフォローアップできるよう、フラグを設定できます。 サポートされているアイテムには、[メッセージ](message.md)と[連絡先](contact.md)があります。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|フォローアップが終了した日時。|
|dueDateTime|**dateTimeTimeZone**|フォローアップが終了する予定の日時。|
|FlagStatus|String|アイテムのフォローアップ状態。 可能な値は、`notFlagged`、`complete`、`flagged` です。|
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
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
