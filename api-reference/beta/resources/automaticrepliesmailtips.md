---
title: automaticRepliesMailTips リソースの種類
description: メールボックスに設定されている自動応答に関するメールヒント。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 74fda9db7de1a97ce2b7e44ca9d56020b87ab6f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974250"
---
# <a name="automaticrepliesmailtips-resource-type"></a>automaticRepliesMailTips リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

メールボックスに設定されている自動応答に関する[メールヒント](../resources/mailtips.md)。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:-----|:-----|:-----|
| メッセージ​​ | String | 自動応答メッセージ。 |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | 自動応答メッセージが含まれる言語。 |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 自動応答を終了する日付と時刻を指定します。 |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 自動応答が開始される日付と時刻。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
