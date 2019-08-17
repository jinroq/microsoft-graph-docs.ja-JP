---
title: activityStatistics リソースの種類
description: 電子メール、会議、フォーカス作業、チャット、通話など、作業活動に費やした時間を表します。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cee94c1ff36bf30d977b7eb97d77f11d4d2ff5e
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450787"
---
# <a name="activitystatistics-resource-type"></a>activityStatistics リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーが稼働時間外にさまざまな作業活動に費やした時間を表します。要求で指定された時間範囲 (1 日の集計期間を使用します)。

次の種類の統計情報は、 **activitystatistics**から派生しています。

* [Call](callactivitystatistics.md)
* [チャット](chatactivitystatistics.md)
* [電子メール](emailactivitystatistics.md)
* [ピント](focusactivitystatistics.md)
* [会議](meetingactivitystatistics.md)

### <a name="activity-id-property"></a>アクティビティ id プロパティ

HTTP 要求で、ある期間内の特定の種類のアクティビティ統計を取得するには、この情報を次の形式`{startdate}`でユーザーの activitystatistics コレクションの ID として表すことができ`{enddate}`ます。ここで、は ISO 8601 カレンダーで表現されています。日付形式と`{activity}`は、"call"、"チャット"、"email"、"focus"、"meeting" のいずれかです。

```
{activity}_{startdate}_{enddate}
```

たとえば、ID が "email_2019-08-10 _2019-08-12" の場合は、指定したユーザーの emailActivityStatistics を2019年8月10日から2019年8月12日まで表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [ActivityStatistics の取得](../api/activitystatistics-get.md) | [activityStatistics](activitystatistics.md) | 指定した時間範囲の、ユーザーに対して指定されたアクティビティの統計のプロパティを取得します。 |
| [ActivityStatistics のリスト](../api/activitystatistics-list.md) | [activityStatistics](activitystatistics.md) | 先週までのユーザーのアクティビティ統計のコレクションのプロパティを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|activity|分析| 統計が返されるアクティビティの種類。 使用可能な値は`call`、 `chat` `email`、、 `focus`、、 `meeting`です。|
|duration|期間|活動に費やした合計時間。 この値は、期間の ISO 8601 形式で表されます。|
|endDate|日付|暦の日付に対して ISO 8601 形式で表された、アクティビティが終了した日付。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-03" にすることができます。|
|id|String| を表す`{activity}_{startdate}_{enddate}`、アクティビティの読み取り専用 ID。|
|startDate|Date|暦の日付に対して ISO 8601 形式で表された、アクティビティが開始された日付。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-04" にすることができます。|
|timeZoneUsed|String|ユーザーが Microsoft Outlook で設定したタイムゾーンが計算に使用されます。 たとえば、プロパティの値は "太平洋標準時" になります。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- { 
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityStatistics",
  "keyProperty": "id"
}-->

```json
{
  "activity": "String",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601 format)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601 format)",
  "timeZoneUsed": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}--> 