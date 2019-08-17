---
title: emailActivityStatistics リソースの種類
description: ユーザーの電子メールアクティビティに関する追加情報を表します。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ff75545b7f591a920ed4a1ffd65bff40cff8439b
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450791"
---
# <a name="emailactivitystatistics-resource-type"></a>emailActivityStatistics リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Outlook での電子メールアクティビティにかかったユーザーの時間に関するデータを表します。 これは、 [Activitystatistics](../resources/activitystatistics.md)に基づいています。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|activity|分析| 統計が返される電子メールアクティビティ。|
|duration|期間|メールに費やした合計時間。 この値は、期間の ISO 8601 形式で表されます。|
|endDate|日付|電子メールアクティビティが終了した日付。 この値は、カレンダーの日付に ISO 8601 形式で表されます。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-04" にすることができます。|
|id|String| 電子メールアクティビティの読み取り専用 ID。|
|startDate|Date|電子メールアクティビティが開始された日付。 この値は、カレンダーの日付に ISO 8601 形式で表されます。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-03" にすることができます。|
|timeZoneUsed|String|ユーザーが Outlook 予定表で設定したタイムゾーンが計算に使用されます。 たとえば、プロパティの値は "太平洋標準時" になります。|
|afterHours|期間|勤務時間外にメールに費やした総時間数。これは、ユーザーの勤務時間に対する Outlook の予定表の設定に基づきます。 この値は、期間の ISO 8601 形式で表されます。 |
|readEmail|期間|電子メールの読み取りにかかった合計時間。 この値は、期間の ISO 8601 形式で表されます。|
|送信メール|期間|電子メールの作成と送信にかかった合計時間。 この値は、期間の ISO 8601 形式で表されます。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailActivityStatistics"
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
  "readEmail": "String (ISO 8601 duration)",
  "sentEmail": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->