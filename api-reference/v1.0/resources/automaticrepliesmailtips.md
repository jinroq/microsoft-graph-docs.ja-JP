---
title: automaticRepliesMailTips リソースの種類
description: メールボックスに設定されている自動応答に関するメールヒント。
localization_priority: Normal
ms.openlocfilehash: bb477979b975996f70e4b8ac624befab7f254f46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569453"
---
# <a name="automaticrepliesmailtips-resource-type"></a>automaticRepliesMailTips リソースの種類


メールボックスに設定されている自動応答に関する[メールヒント](../resources/mailtips.md)。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:-----|:-----|:-----|
| メッセージ​​ | String | 自動応答メッセージ。 |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | 自動応答メッセージが含まれる言語。 |
| scheduledendtime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 自動応答を終了する日付と時刻を指定します。 |
| scheduledstarttime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 自動応答が開始される日付と時刻。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
