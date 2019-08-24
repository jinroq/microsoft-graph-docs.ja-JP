---
title: chatActivityStatistics リソースの種類
description: ユーザーのチャット活動に関する情報を表します。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 05003110c397932f27e700c119f3926b44fe7c31
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622643"
---
# <a name="chatactivitystatistics-resource-type"></a>chatActivityStatistics リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams または Skype for Business でのチャット活動にかかったユーザーの時間に関するデータを表します。 これは、 [Activitystatistics](../resources/activitystatistics.md)に基づいています。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|activity|分析| 統計が返されるチャットアクティビティ。|
|duration|期間|チャットに費やした合計時間。 この値は、期間の ISO 8601 形式で表されます。|
|endDate|日付|チャットアクティビティが終了した日付。 この値は、カレンダーの日付に ISO 8601 形式で表されます。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-04" にすることができます。|
|id|String| チャットアクティビティの読み取り専用 ID。|
|startDate|Date|チャットアクティビティが開始された日付。 この値は、カレンダーの日付に ISO 8601 形式で表されます。 たとえば、プロパティの値は、YYYY-MM-DD 形式の "2019-07-03" にすることができます。|
|timeZoneUsed|String|ユーザーが Outlook 予定表で設定したタイムゾーンが計算に使用されます。 たとえば、プロパティの値は "太平洋標準時" になります。|
|afterHours|期間|就業時間外のチャットに費やした時間。これは、ユーザーの勤務時間に対する Microsoft Outlook の予定表の設定に基づきます。 この値は、期間の ISO 8601 形式で表されます。 |

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatActivityStatistics"
}-->

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)"
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

