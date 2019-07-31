---
title: accessReviewSettings リソースの種類
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 2c51d94b3143d9929c03093cfb1a6625d6a9e3db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974538"
---
# <a name="accessreviewsettings-resource-type"></a>accessReviewSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
| mailNotificationsEnabled | ブール値 |  |
| remindersEnabled | ブール値 |  |
| justificationRequiredOnApproval | ブール値 |  |
| recurrenceSettings | accessReviewRecurrenceSettings |  |
| autoReviewEnabled | ブール値 |  |
| activityDurationInDays | Int32 |  |
| autoReviewSettings | autoReviewSettings |  |
| autoApplyReviewResultsEnabled | ブール値 |  |
| accessRecommendationsEnabled | ブール値 |  |


## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
``` json
{
    "mailNotificationsEnabled":"boolean",
    "remindersEnabled":"boolean",
    "justificationRequiredOnApproval":"boolean",
    "recurrenceSettings":"microsoft.graph.accessReviewRecurrenceSettings",
    "autoReviewEnabled":"boolean",
    "activityDurationInDays":"Int32",
    "autoReviewSettings":"microsoft.graph.autoReviewSettings",
    "autoApplyReviewResultsEnabled":"boolean",
    "accessRecommendationsEnabled":"boolean"
}
```



