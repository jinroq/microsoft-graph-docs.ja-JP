---
title: 会議 Activitystatistics リソースの種類
description: ユーザーの会議活動に関する情報を表します。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa0e4b12ed260c0f6660544e7f48cfe1ca9cd3dc
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450789"
---
# <a name="meetingactivitystatistics-resource-type"></a>会議 Activitystatistics リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Outlook、Microsoft Teams、または Skype for Business の会議に費やしたユーザーの時間に関するデータを表します。 これは、 [Activitystatistics](../resources/activitystatistics.md)に基づいています。
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|activity|分析| 統計が返される会議アクティビティ。|
|duration|期間|会議に費やした合計時間。 この値は、期間の ISO 8601 形式で表されます。|
|endDate|日付|会議の活動が終了した日付。 この値は、カレンダーの日付に ISO 8601 形式で表されます。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-04" にすることができます。|
|id|String| 会議アクティビティの読み取り専用 ID。|
|startDate|Date|会議の活動が開始された日付。 この値は、カレンダーの日付に ISO 8601 形式で表されます。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-03" にすることができます。|
|timeZoneUsed|String|Outlook の予定表にユーザーが設定した Outlook タイムゾーンが計算に使用されます。 たとえば、プロパティの値は "太平洋標準時" になります。|
|afterHours|期間|勤務時間外の会議に費やした時間。これは、ユーザーの勤務時間に対する Outlook の予定表の設定に基づいています。 この値は、期間の ISO 8601 形式で表されます。|
|い|期間|競合する会議 (相手が承諾した会議と、ユーザーの状態が [取り込み中] に設定されている他の会議と重複する会議) にかかった時間。 この値は、期間の ISO 8601 形式で表されます。|
|long|期間|長時間の会議でかかった時間 (時間で1時間以上)。 この値は、期間の ISO 8601 形式で表されます。|
|マルチタスク|期間|ユーザーがマルチタスクを行った会議 (少なくとも、少なくとも1つのメール、または Teams または Skype for Business の少なくとも1つのメッセージ数を超える) にかかった時間。 この値は、期間の ISO 8601 形式で表されます。|
|別|期間|ユーザーが開催した会議にかかった時間。 この値は、期間の ISO 8601 形式で表されます。|
|予定|期間|定期的な会議に費やした時間。 この値は、期間の ISO 8601 形式で表されます。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "conflicting": "String (ISO 8601 duration)",
  "long": "String (ISO 8601 duration)",
  "multitasking": "String (ISO 8601 duration)",
  "organized": "String (ISO 8601 duration)",
  "recurring": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->