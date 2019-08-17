---
title: focusActivityStatistics リソースの種類
description: ユーザーの個々のフォーカス作業に関する情報を表します。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fc4431ac20c961569ce5cfaa607c2d2ab77240ee
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450780"
---
# <a name="focusactivitystatistics-resource-type"></a>focusActivityStatistics リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

フォーカス作業に使用できるユーザーの時間に関するデータを表します。 これは、 [Activitystatistics](../resources/activitystatistics.md)に基づいています。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|activity|分析| 統計が返されるフォーカスアクティビティ。|
|duration|期間|ユーザーの勤務時間内の他のユーザーとの会議を行わずに、ユーザーの Microsoft Outlook の予定表にある、少なくとも2つの連続する時間のすべての時間ブロックに等しい合計フォーカス時間の合計。 この値は、期間の ISO 8601 形式で表されます。|
|endDate|日付|フォーカスアクティビティが終了した日付。 この値は、カレンダーの日付に ISO 8601 形式で表されます。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-04" にすることができます。|
|id|String| フォーカスアクティビティの読み取り専用 ID。|
|startDate|Date|フォーカスアクティビティが開始された日付。 この値は、カレンダーの日付に ISO 8601 形式で表されます。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-03" にすることができます。|
|timeZoneUsed|String|ユーザーが Outlook 予定表で設定したタイムゾーンが計算に使用されます。 たとえば、プロパティの値は "太平洋標準時" になります。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.focusActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String"
  }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "focusActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->