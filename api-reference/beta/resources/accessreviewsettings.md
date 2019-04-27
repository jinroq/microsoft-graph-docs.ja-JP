---
title: accessReviewSettings リソースの種類
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348406"
---
# <a name="accessreviewsettings-resource-type"></a>accessReviewSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
| mailNotificationsEnabled | boolean |  |
| remindersEnabled | boolean |  |
| justificationRequiredOnApproval | boolean |  |
| recurrenceSettings | accessReviewRecurrenceSettings |  |
| autoreviewenabled | boolean |  |
| activityDurationInDays | Int32 |  |
| autoreviewsettings | autoreviewsettings |  |
| autoApplyReviewResultsEnabled | boolean |  |
| accessRecommendationsEnabled | boolean |  |


## <a name="relationships"></a>関係
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



